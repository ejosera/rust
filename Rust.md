# Rust

## Documentation
https://doc.rust-lang.org/book/ch00-00-introduction.html
https://github.com/rust-lang/book/tree/main/src

## description
a
## Developer tools
- Cargo: the included dependency manager and build tool
- rustfmt: formatting
- The Rust Language Server: IDE

## Install
```bash
curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh
info: downloading installer

Welcome to Rust!

This will download and install the official compiler for the Rust
programming language, and its package manager, Cargo.

Rustup metadata and toolchains will be installed into the Rustup
home directory, located at:

  /home/jose/.rustup

This can be modified with the RUSTUP_HOME environment variable.

The Cargo home directory is located at:

  /home/jose/.cargo

This can be modified with the CARGO_HOME environment variable.

The cargo, rustc, rustup and other commands will be added to
Cargo's bin directory, located at:

  /home/jose/.cargo/bin

This path will then be added to your PATH environment variable by
modifying the profile files located at:

  /home/jose/.profile
  /home/jose/.bashrc

You can uninstall at any time with rustup self uninstall and
these changes will be reverted.

Current installation options:


   default host triple: x86_64-unknown-linux-gnu
     default toolchain: stable (default)
               profile: default
  modify PATH variable: yes

1) Proceed with standard installation (default - just press enter)
2) Customize installation
3) Cancel installation
>

info: profile set to 'default'
info: default host triple is x86_64-unknown-linux-gnu
info: syncing channel updates for 'stable-x86_64-unknown-linux-gnu'
info: latest update on 2025-12-11, rust version 1.92.0 (ded5c06cf 2025-12-08)
info: downloading component 'cargo'
 10.3 MiB /  10.3 MiB (100 %)   9.3 MiB/s in  1s         
info: downloading component 'clippy'
info: downloading component 'rust-docs'
 20.5 MiB /  20.5 MiB (100 %)  10.0 MiB/s in  2s         
info: downloading component 'rust-std'
 28.0 MiB /  28.0 MiB (100 %)   8.9 MiB/s in  3s         
info: downloading component 'rustc'
 74.3 MiB /  74.3 MiB (100 %)  10.0 MiB/s in  8s         
info: downloading component 'rustfmt'
info: installing component 'cargo'
info: installing component 'clippy'
info: installing component 'rust-docs'
 20.5 MiB /  20.5 MiB (100 %)   5.8 MiB/s in  3s         
info: installing component 'rust-std'
 28.0 MiB /  28.0 MiB (100 %)   9.7 MiB/s in  2s         
info: installing component 'rustc'
 74.3 MiB /  74.3 MiB (100 %)  10.6 MiB/s in  6s         
info: installing component 'rustfmt'
info: default toolchain set to 'stable-x86_64-unknown-linux-gnu'

  stable-x86_64-unknown-linux-gnu installed - rustc 1.92.0 (ded5c06cf 2025-12-08)


Rust is installed now. Great!

To get started you may need to restart your current shell.
This would reload your PATH environment variable to include
Cargo's bin directory ($HOME/.cargo/bin).

To configure your current shell, you need to source
the corresponding env file under $HOME/.cargo.

This is usually done by running one of the following (note the leading DOT):
. "$HOME/.cargo/env"            # For sh/bash/zsh/ash/dash/pdksh
source "$HOME/.cargo/env.fish"  # For fish
source $"($nu.home-path)/.cargo/env.nu"  # For nushell
```

Compruebo la versión
```bash
rustc --version
rustc 1.92.0 (ded5c06cf 2025-12-08)
```

## Actualizo rust
rustup update

## Desisntalo rust
rustup self uninstall

## documentación
rustup doc

## hello world
```bash
fn main() {
    println!("Hello, world!");
}
```
println es una función
println! en una macro

## Ejecución
rustc main.rs
./main

## cargo
Es una herramienta para gestionar la dependencias y compilasr rust
```bash
cargo new hello_cargo
cd hello_cargo
```

Ha creado 
- un archivo proyecto .toml
- un directorio src
  - mail.rs

Compilo en desarrollo
cargo build

Compilo en producción (mas rendimiento)
cargo build --release

Compilo y ejecuto
cargo run

Compruebo
cargo check