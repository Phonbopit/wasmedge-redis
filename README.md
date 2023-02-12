# Hello WASM Edge Redis

## Usage

1. Install WasmEdge

```
curl -sSf https://raw.githubusercontent.com/WasmEdge/WasmEdge/master/utils/install.sh | bash
```

2. Run a demo

```
cargo build --target wasm32-wasi --release
wasmedge --env "REDIS_URL=redis://localhost/" target/wasm32-wasi/release/wasmedge-redis.wasm
```

> Note: Please don't forget to change your package name `wasmedge-redis` to your app name.

## Reference

- https://github.com/WasmEdge/wasmedge-db-examples
