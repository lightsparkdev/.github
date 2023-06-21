# ⚡️ Hi, we're Lightspark!

![Github_Header](https://github.com/lightsparkdev/.github/assets/1393755/d91d8c57-e8d1-4588-8289-26ef9da73e9e)

The Lightning Network is an open, low cost, interoperable payment network that settles in real time. Lightspark is the easiest, most reliable, enterprise-grade gateway to Lightning, enabling money to move just like bits and bytes do on the Internet. You can learn more about our products [here](https://www.lightspark.com/products).

**Welcome to our github home!** Here you'll find our open-source SDKs that you can use to enable Lightning payments in your app, website, or backend. You can find full documentation for our SDKs and APIs [📃 here](https://app.lightspark.com/docs). Here's a summary of some of the repositories you'll find in our org:

## ![typescript](https://github.com/lightsparkdev/.github/assets/1393755/0ad3c4db-5938-4c69-9a30-c99399c0330d) [js-sdk](https://github.com/lightsparkdev/js-sdk)

This repository contains all of the Lightspark Javascript/Typescript SDKs. Some of the included npm packages are:

- [lightspark-sdk](https://github.com/lightsparkdev/js-sdk/tree/main/packages/lightspark-sdk/README.md): A high-level management SDK that can be used from a node or browser environment. It's used to manage accounts, nodes, wallets, etc. and should be authenticated via API token or OAuth.
- [wallet-sdk](https://github.com/lightsparkdev/js-sdk/tree/main/packages/wallet-sdk/README.md): A client-side wallet SDK, which can be used from a browser or React Native environment. It's meant to interact with a single wallet user.
- [react-wallet](https://github.com/lightsparkdev/js-sdk/tree/main/packages/react-wallet/README.md): A React library that wraps the wallet SDK and provides some convenient React hooks.
- [react-native](https://github.com/lightsparkdev/js-sdk/tree/main/packages/react-native): Utilities and alternative implementations of some core Lightspark SDK interfaces to add compatibility with react-native.
- A few other small utility packages

Check out the READMEs for each package for more information on how to use them, or see the `examples` directory in each package for sample use cases.

## 🍎 [swift-wallet-sdk](https://github.com/lightsparkdev/swift-wallet-sdk)

This is a Swift Wallet SDK for the Lightspark Wallet APIs. It can be used from an iOS environment to integrate with a Lightspark Lightning wallet. It also contains a demo iOS app to show how to use the SDK. You can also check out its [documentation](https://app.lightspark.com/docs/wallet-sdk/getting-started) or [API Reference](https://lightsparkdev.github.io/swift-wallet-sdk/documentation/lightsparkwallet/).

## 🤖 [kotlin-sdk](https://github.com/lightsparkdev/kotlin-sdk)

This repository contains the Lightspark Kotlin (multiplatform) SDKs. They can be used from either Kotlin or Java, from Android or another JVM context. The repository also contains a sample Android app which uses the wallet-sdk to display basic node, channel, and transaction information. Modules are published to maven-central. Important modules include:

- [lightspark-sdk](https://github.com/lightsparkdev/kotlin-sdk/tree/main/lightspark-sdk/README.md): A simple wrapper around the Lightspark GraphQL server API. It's used to manage accounts, nodes, wallets, etc. It can authenticate using an Account API token retrieved from your Lightspark account dashboard or via the oauth module.
- [wallet-sdk](https://github.com/lightsparkdev/kotlin-sdk/tree/main/wallet-sdk/README.md): An SDK for interacting with the Lightspark API for a single wallet user. See its [documentation](https://app.lightspark.com/docs/wallet-sdk/getting-started) or [API Reference](https://app.lightspark.com/docs/reference/kotlin/wallet-sdk/index.html). It can be used from an Android environment and is used by the sample app [androidWalletDemo](https://github.com/lightsparkdev/kotlin-sdk/tree/main/androidwalletdemo). See its README for more info.
- [core](https://github.com/lightsparkdev/kotlin-sdk/tree/main/core). A module containing common utilities for networking, authentication, and more.
- There are also a few other small utility modules.

## 🛠️ Lightspark SDK for other languages

In addition to JS and Kotlin/Java, we also offer the [Lightspark SDK](https://app.lightspark.com/docs/api/2023-04-04/getting-started) in **[Rust](https://github.com/lightsparkdev/lightspark-rs), [Python](https://github.com/lightsparkdev/python-sdk), and [Golang](https://github.com/lightsparkdev/go-sdk)**. See the README file for your language or choice, and check out our [API Docs](https://app.lightspark.com/docs/api/2023-04-04/getting-started) to get started.

