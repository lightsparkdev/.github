# Hi, we're Lightspark!

![Github_Header](https://github.com/lightsparkdev/.github/assets/1393755/d91d8c57-e8d1-4588-8289-26ef9da73e9e)

The Lightning Network is an open, low cost, interoperable payment network that settles in real time. Lightspark is the easiest, most reliable, enterprise-grade gateway to Lightning, enabling money to move just like bits and bytes do on the Internet. You can learn more about our products [here](https://www.lightspark.com/products).

**Welcome to our github home!** Here you'll find our open-source SDKs that you can use to enable Lightning payments in your app, website, or backend. You can find full documentation for our SDKs and APIs [📃 here](https://app.lightspark.com/docs). Here's a summary of some of the repositories you'll find in our org:

## [Lightspark SDK](https://docs.lightspark.com/lightspark-sdk/getting-started)
Our Lightspark SDK is the quickest and most cost-effective way to send and receive Bitcoin payments on the Lightning Network. It is available in several programming languages:

- [Typescript](https://github.com/lightsparkdev/js-sdk/tree/main/packages/lightspark-sdk/README.md) ([docs](https://docs.lightspark.com/lightspark-sdk/getting-started?language=typescript))
- [Python](https://github.com/lightsparkdev/python-sdk) ([docs](https://docs.lightspark.com/lightspark-sdk/getting-started?language=python))
- [Golang](https://github.com/lightsparkdev/go-sdk) ([docs](https://docs.lightspark.com/lightspark-sdk/getting-started?language=go))
- [Rust](https://github.com/lightsparkdev/lightspark-rs) ([docs](https://docs.lightspark.com/lightspark-sdk/getting-started?language=rust))
- [Kotlin, Java, and other JVM Languages](https://github.com/lightsparkdev/kotlin-sdk/tree/main/lightspark-sdk/README.md) ([Kotlin docs](https://docs.lightspark.com/lightspark-sdk/getting-started?language=kotlin)) ([Java docs](https://docs.lightspark.com/lightspark-sdk/getting-started?language=java))

Check out the READMEs for each package for more information on how to use them, or see the `examples` directory in each package for sample use cases.

## 🤖 [UMA Demo VASPs](https://docs.lightspark.com/uma-sdk/introduction?language=typescript)

[UMA](https://docs.uma.me) lets anyone send and receive money (fiat and crypto) 24/7 using their favorite UMA-enabled wallet, exchange, or bank. The main UMA protocol definition and SDK implementations are in the [UMA Github org](https://github.com/uma-universal-money-address). However, this repo contains some useful demo VASP implementations that use the Lightspark SDK for lightning payments.

- [Golang VASP using Gin](https://github.com/lightsparkdev/go-sdk/tree/main/examples/uma-server)
- [Python VASP using Flask](https://github.com/lightsparkdev/uma-demo-vasp-python)
- [Typescript VASP using express](https://github.com/lightsparkdev/js-sdk/tree/main/apps/examples/uma-vasp)
- [Kotlin VASP using ktor](https://github.com/lightsparkdev/kotlin-sdk/tree/develop/umaserverdemo)

## 🛠️ Other small utility repos

- [lightspark-crypto-uniffi](https://github.com/lightsparkdev/lightspark-crypto-uniffi) - A rust library for many low-level crypto operations used by several Lightspark SDK implementations in various languages.
- [compose-qr-code](https://github.com/lightsparkdev/compose-qr-code) - A simple, flexible QR code renderer for Jetpack Compose

