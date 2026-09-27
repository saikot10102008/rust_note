**Constants in Rust – Complete Notes**

Constants are used to store values that **never change**.

Unlike regular variables, constants **must** be defined with a type (for example `i32` or `char`).

### Creating a Constant

To create a constant, use the `const` keyword, followed by the name, the type, and the value:

```rust
const BIRTHYEAR: i32 = 1980;

const MINUTES_PER_HOUR: i32 = 60;
```

### Constants Must Have a Type

You must always write the type when creating a constant.  
You cannot let Rust guess the type the way you can with regular variables:

```rust
const BIRTHYEAR: i32 = 1980; // Correct

const BIRTHYEAR = 1980;      // Error: missing type
```

### Naming Rules

It is considered good practice to write constant names in **uppercase**.

This is not required by the language, but it improves readability and is the common style used by Rust programmers.

Examples of good constant names:
- `MAX_SPEED`
- `PI`
- `MINUTES_PER_HOUR`

### Constants vs Variables – Quick Comparison

| Feature          | Constant (`const`)          | Variable (`let`)              |
|------------------|-----------------------------|-------------------------------|
| Can change?      | No                          | Yes, if `mut` is used         |
| Type required?   | Yes                         | No (optional)                 |

Constants are perfect for values that should stay the same throughout the entire program, such as mathematical constants, configuration limits, or fixed numbers.
