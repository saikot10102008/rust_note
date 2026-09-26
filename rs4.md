**Printing Text in Rust**

In Rust, you display text (output) using special tools called **macros**. The main one for beginners is `println!`.

### Using `println!`
The `println!` macro prints text and automatically moves to a new line afterward.

```rust
println!("Hello World!");
```

You can use it as many times as you want. Each call starts on a new line:

```rust
println!("Hello World!");
println!("I am learning Rust.");
println!("It is awesome!");
```

**Output:**
```
Hello World!
I am learning Rust.
It is awesome!
```

### Using `print!`
There is a similar macro called `print!`. It works almost the same way, but it **does not** add a new line at the end.

```rust
print!("Hello World! ");
print!("I will print on the same line.");
```

**Output:**
```
Hello World! I will print on the same line.
```

Notice the extra space after `"Hello World!"` — you often need to add spaces yourself so the text looks readable.

Most examples use `println!` because the output is easier to read.

### Adding New Lines Manually with `\n`
If you want a new line while using `print!`, insert the special character `\n` (called a **newline character** or **escape sequence**).

```rust
print!("Hello World!\n");
print!("I will print on the same line.");
```

You can also place `\n` in the middle of a string with either macro:

```rust
println!("Hello World!\nThis line was broken up!");
```

**Output:**
```
Hello World!
This line was broken up!
```

`\n` forces the cursor to jump to the beginning of the next line on the screen.

### Quick Summary for Beginners
| Macro       | Adds new line? | Common use                          |
|-------------|----------------|-------------------------------------|
| `println!`  | Yes            | Most everyday printing              |
| `print!`    | No             | When you want text on the same line |

These macros are the basic way to show messages, results, or any text while learning Rust.
