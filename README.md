# rust.redis.web

An example of using Redis in a Rust web application implementing three different ways to use 
redis within a warp web service:

* [redis-rs without a pool](https://github.com/mitsuhiko/redis-rs) 
* [mobc](https://github.com/importcjj/mobc)
* [r2d2](https://github.com/sorccu/r2d2-redis)

## Getting Started

To run the application in dev mode:

1. Start the redis instance:

```bash
docker run -p 6379:6379 redis:6.0
```

2. Starting the application:

```bash
make dev
```

3. Test the different endpoints using:

```bash
curl http://localhost:8080/mobc
mobc_world

curl http://localhost:8080/r2d2
r2d2_world

curl http://localhost:8080/direct
direct_world
```
