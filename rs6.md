**Variables in Rust**

Variables are containers that store data values, such as numbers or text.

### Creating a Variable
Use the `let` keyword followed by a name and a value:

```rust
let name = "John";
println!("My first name is: {}", name);
```

**Output:**  
`My first name is: John`

### The `{}` Placeholder
Rust uses `{}` inside `println!` as a placeholder. The value of the variable is inserted in place of `{}`.

You can use multiple placeholders:

```rust
let name = "John";
let age = 30;
println!("{} is {} years old.", name, age);
```

**Output:**  
`John is 30 years old.`

The values are placed in the same order you list them after the string:
- First `{}` gets the first value (`name`)
- Second `{}` gets the second value (`age`)

**Important:** Order matters. If you switch the values, the output changes:

```rust
let name = "John";
let age = 30;
println!("{} is {} years old.", age, name);
// Outputs: 30 is John years old
```

### Variables Are Immutable by Default
By default, once you create a variable, you **cannot** change its value:

```rust
let x = 5;
x = 10; // This causes an error
println!("{}", x);
```

### Making a Variable Mutable (Changeable)
If you need to change a variable’s value later, add the `mut` keyword (short for *mutable*):

```rust
let mut x = 5;
println!("Before: {}", x);

x = 10;
println!("After: {}", x);
```

**Output:**  
```
Before: 5
After: 10
```

### Quick Summary
| Keyword     | Meaning                          | Example              |
|-------------|----------------------------------|----------------------|
| `let`       | Create a variable (immutable)    | `let x = 5;`         |
| `let mut`   | Create a changeable variable     | `let mut x = 5;`     |
| `{}`        | Placeholder for variable values  | `println!("{}", x);` |

This is the foundation of storing and displaying data in Rust.
