# buildkit-setup

Composite action that wires up `docker/setup-buildx-action` against the shared
rootless buildkitd in the `tooling-prod` EKS cluster. Use on any ARC runner
before `docker/build-push-action`.

## Usage

```yaml
jobs:
  build:
    runs-on: arc-runner-4
    steps:
      - uses: actions/checkout@v4
      - uses: lightsparkdev/.github/actions/buildkit-setup@v1
      - uses: docker/build-push-action@v6
        with:
          context: .
          push: true
          tags: ...
```

That's it. No `setup-buildx-action` call of your own, no per-workflow TLS
plumbing. The runner pod has the mTLS client cert mounted at
`/etc/buildkit-client/{ca,tls.crt,tls.key}` (handled by the gha-runner-scale-set
chart in `lightsparkdev/tooling-infra`).

## Inputs

| Name       | Default                                                            | Notes                                                                                                              |
|------------|--------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------|
| `endpoint` | `tcp://buildkitd.buildkit.svc.cluster.local:1234`                  | Override for testing against a specific replica via per-pod DNS (`buildkitd-N.buildkitd.buildkit.svc.cluster.local`). |

## Where this works

- `runs-on: arc-runner-{1,2,4,8}` — the in-cluster ARC scale sets.
- Not GH-hosted runners (the buildkit service is cluster-internal; the certs aren't there).

## When NOT to use this

- Workflows that need `services:` blocks (postgres, redis, etc.) — those need a real docker daemon, not just buildx.
- `kind`/`tilt`-based hermetic tests — same reason. These should stay on GH-hosted.
