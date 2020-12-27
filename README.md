# libmdns - Rust mDNS responder

libmdns is a pure rust implementation of the mDNS ([RFC 6762]) and DNS-SD ([RFC 6763]) protocols.

[RFC 6762]: https://tools.ietf.org/html/rfc6762
[RFC 6763]: https://tools.ietf.org/html/rfc6763

## Usage

To use it, add this to your `Cargo.toml`:

```toml
[dependencies]
libmdns = "0.6"
```

See the [example](https://github.com/librespot-org/libmdns/blob/stable-0.6.x/examples/register.rs) for use within code.

## Dependencies

**Only the latest stable version of rust and cargo are officially supported for now.**
Please open an issue on GitHub if you need support for older versions.

libmdns is built with the help of the [tokio](https://github.com/tokio-rs/tokio) runtime.

* `libmdns 0.6.x` (`tokio=1.x`, `rustc>=1.45.2`)
* `libmdns 0.5.x` (`tokio=0.3`, `rustc>=1.45.2`)
* `libmdns 0.4.x` (`tokio=0.2`, `rustc>=1.40.0`)
* `libmdns 0.3.x` (`tokio=0.1`, `rustc>=1.40.0`)
* `libmdns 0.2.x` (`tokio-core=0.1`, `rustc>=1.40.0`)

_May compile fine on older versions of rust, but the minimum garaunteed version is listed as above._

## Provenance Note
This project originally started as a fork of [plietar/rust-mdns](https://github.com/plietar/rust-mdns).
