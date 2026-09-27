**Data Types in Rust – Complete Notes**

In Rust, variables do **not** need to be declared with a specified type (unlike languages such as C or Java where you write “String” or “Int”).

Rust looks at the value you give the variable and automatically chooses the correct type:

```rust
let my_num = 5;         // integer
let my_double = 5.99;   // float
let my_letter = 'D';    // character
let my_bool = true;     // boolean
let my_text = "Hello";  // string
```

You can also **explicitly** tell Rust the type if you want:

```rust
let my_num: i32 = 5;          // integer
let my_double: f64 = 5.99;    // float
let my_letter: char = 'D';    // character
let my_bool: bool = true;     // boolean
let my_text: &str = "Hello";  // string
```

It is good to understand what the different types mean, even if you don’t always write them yourself.

### Basic Data Types Are Divided into These Groups

- **Numbers** – Whole numbers and decimal numbers (`i32`, `u32`, `f64`)
- **Characters** – Single letters or symbols (`char`)
- **Strings** – Text, a sequence of characters (`&str`)
- **Booleans** – True or false values (`bool`)

---

### Numbers

Number types are divided into two groups: **integer types** and **floating-point types**.

#### Integers (`i32` and `u32`)

Integer types store whole numbers without decimals.

Two common integer types:

- `i32` → can store **positive and negative** whole numbers  
- `u32` → can only store **zero or positive** whole numbers

```rust
let temperature: i32 = -5;
let age: u32 = 25;

println!("Temperature: {}", temperature);
println!("Age: {}", age);
```

The `u` in `u32` means **unsigned**, which means the value cannot be negative.  
This makes `u32` useful for values such as age, counts, and sizes.

#### Floating Point (`f64`)

The `f64` type is used to store numbers that contain one or more decimals:

```rust
let price: f64 = 19.99;
println!("Price is: ${}", price);
```

---

### Characters (`char`)

The `char` type stores a **single** character.  
A `char` value must be surrounded by **single quotes** (`'`).

```rust
let my_grade: char = 'B';
println!("{}", my_grade);
```

---

### Strings (`&str`)

The `&str` type stores a **sequence of characters** (text).  
String values must be surrounded by **double quotes** (`"`).

```rust
let name: &str = "John";
println!("Hello, {}!", name);
```

---

### Booleans (`bool`)

The `bool` type can only take the values `true` or `false`:

```rust
let is_logged_in: bool = true;
println!("User logged in? {}", is_logged_in);
```

---

### Combining Data Types

You can freely mix different types in the same program:

```rust
let name = "John";
let age = 28;
let is_admin = false;

println!("Name: {}", name);
println!("Age: {}", age);
println!("Admin: {}", is_admin);
```

---

### Quick Summary Table

| Type   | What it stores                        | Example          | Quotes needed?   |
|--------|---------------------------------------|------------------|------------------|
| `i32`  | Whole numbers (positive & negative)   | `-5`, `42`       | None             |
| `u32`  | Whole numbers (0 or positive only)    | `25`, `100`      | None             |
| `f64`  | Numbers with decimals                 | `19.99`          | None             |
| `char` | Single character                      | `'A'`, `'B'`     | Single quotes    |
| `&str` | Text / string of characters           | `"Hello"`        | Double quotes    |
| `bool` | True or false                         | `true`, `false`  | None             |

These are the fundamental data types you will use when storing information in Rust.
