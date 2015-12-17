# rust-multiaddr

[![Build Status](https://img.shields.io/travis/Dignifiedquire/rust-multiaddr/master.svg?style=flat-square)](https://travis-ci.org/Dignifiedquire/rust-multiaddr)
[![](https://img.shields.io/badge/docs-blue.svg?style=flat-square)](http://dignifiedquire.github.io/rust-multiaddr/multiaddr/struct.Multiaddr.html)

> [multiaddr](https://github.com/jbenet/multiaddr) implementation in Rust.


## Usage

First add this to your `Cargo.toml`

```toml
[dependencies]
multiaddr = "*"
```

```rust
crate extern multiaddr

use multiaddr::Multiaddr;

let address = Multiaddr::new("/ip4/127.0.0.1/udp/1234").unwrap();

assert_eq!(address.to_string(), "/ip4/127.0.0.1/udp/1234");
```


## License

[MIT](LICENSE)
