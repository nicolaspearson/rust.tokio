# rust.tokio

This repository contains completed tutorials from [Tokio](https://tokio.rs/tokio/tutorial).

## Getting Started

To run the application in dev mode:

1. Install the Mini-Redis server:

```bash
$ cargo install mini-redis
$ mini-redis-server
```

Then try to get the key `foo` using `mini-redis-cli`:

```bash
$ mini-redis-cli get foo
```

The result should be: `(nil)`.

2. Start the application:

```bash
$ cargo run
```
