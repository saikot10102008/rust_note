**Basic structure of a Rust program**

```rust
fn main() {
    println!("Hello world");
}
```

**Key elements**

- `fn` — Keyword used to define a function.
- `main` — Special function that serves as the entry point. Every executable Rust program starts execution here.
- `{}` — Curly braces define a code block (the body of the function).
- `println!` — Macro that prints text to the console followed by a newline.  
  The `!` indicates it is a macro, not a regular function. Without the `!` it would be treated as a normal function call.
- `"..."` — String literals must use double quotes. Single quotes are not valid for strings.
- `;` — Terminates a statement. Required when multiple statements appear in sequence.

**Example with multiple statements**

```rust
fn main() {
    println!("Hello world");
    println!("Hello Bob");
}
```

Omitting the semicolons between statements causes a compilation error because Rust cannot determine where one statement ends and the next begins.

**Note on the final statement**  
In some contexts the semicolon on the last expression inside a function can be omitted (turning it into an expression that returns a value). For simple printing examples, including the semicolon is the standard and clearest approach.
