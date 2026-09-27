**Installing Rust**

Rust is installed using **rustup**, the official installer and version manager.

- Visit https://www.rust-lang.org/tools/install
- On macOS / Linux: run the provided `curl` command in the terminal and choose the standard installation.
- On Windows: use the standalone installer.

**Verification**:
```bash
rustc --version
```

**First program (manual method)**

Create a file named `main.rs` containing:

```rust
fn main() {
    println!("Hello world");
}
```

- `fn main()` — Entry point of a Rust binary. Program execution begins here.
- `println!` — Macro that prints text to the console followed by a newline. The `!` indicates it is a macro, not a regular function.
- `;` — Terminates a statement.

**Compile**:
```bash
rustc main.rs
```

**Run**:
```bash
./main          # macOS / Linux
.\main.exe      # Windows
```

**Using Cargo**

Cargo is Rust’s build system and package manager. It handles compilation, execution, and project structure.

Create a new project:
```bash
cargo new hello_world
cd hello_world
```

This generates:
- `Cargo.toml` — Project metadata and dependency list
- `src/main.rs` — Source file (pre-populated with a Hello World program)

**Common commands**:
- `cargo build` — Compiles the project
- `cargo run` — Compiles (if needed) and runs the program
- `cargo check` — Checks for errors without producing a binary

`cargo run` is the usual workflow for development because it automatically recompiles after changes.
