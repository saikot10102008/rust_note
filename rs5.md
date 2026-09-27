**Comments in Rust**

Comments are notes you write inside your code. They help explain what the code does, make it easier to read, and can temporarily stop some code from running while you test other ideas.

The Rust compiler completely ignores comments — they never affect how the program works.

There are two main types: single-line and multi-line.

### Single-line Comments
A single-line comment starts with two forward slashes: `//`

Everything after `//` on that line is ignored.

**Example – comment before a line of code:**
```rust
// This is a comment
println!("Hello World!");
```

**Example – comment at the end of a line:**
```rust
println!("Hello World!"); // This is a comment
```

### Multi-line Comments
A multi-line comment starts with `/*` and ends with `*/`.

Everything between these markers is ignored, even if it spans several lines.

**Example:**
```rust
/* The code below will print the words Hello World!
to the screen, and it is amazing */
println!("Hello World!");
```

### Which one should you use?
- Use `//` for short notes.
- Use `/* */` when you need to write longer explanations that take more than one line.

Both styles are correct — choose whichever feels clearer for the situation.
