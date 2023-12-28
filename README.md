<p align=center>
  <b>You're probably looking for <a href="https://jcbhmr-hello-world-rust-wasmer-app.wasmer.app/">jcbhmr-hello-world-rust-wasmer-app.wasmer.app</a></b>
</p>

# "Hello world!" Rust Wasmer app

🟪 "Hello world!" demo [Wasmer] HTTP server application

<p align=center>
  <img src="https://i.imgur.com/WaxzU93.png">
</p>

🟪 Uses Wasmer's new app platform \
🦀 Written in Rust \
🅰 Uses the [Axum] HTTP server library \
👩‍⚖️ [0BSD licensed] template

## Development

![Rust](https://img.shields.io/static/v1?style=for-the-badge&message=Rust&color=000000&logo=Rust&logoColor=FFFFFF&label=)
![WebAssembly](https://img.shields.io/static/v1?style=for-the-badge&message=WebAssembly&color=654FF0&logo=WebAssembly&logoColor=FFFFFF&label=)

Make sure you have the `wasm32-wasi` Rust target installed. You'll also need the
[Wasmer CLI] and [`cargo-wasix`] installed.

Write the backend Rust code _as though_ it were a normal HTTP server. That HTTP
server will compile to WASIX which will then be started by Wasmer's app backend
and have the request forwarded to it. Then after an indeterminate amount of time
it will be killed and stop recieving additional requests.

Note that the version fields all mean **absolutely nothing** in this context. Each
time you run `wasmer deploy`, it will bump the version. That version isn't
exposed anywhere to the endpoint.

<!-- prettier-ignore-start -->
[0BSD licensed]: https://github.com/jcbhmr/hello-world-rust-wasmer-app/blob/main/LICENSE
[wasmer]: https://wasmer.io/
[axum]: https://github.com/tokio-rs/axum
[wasmer cli]: https://docs.wasmer.io/install
[`cargo-wasix`]: https://github.com/wasix-org/cargo-wasix
<!-- prettier-ignore-end -->
