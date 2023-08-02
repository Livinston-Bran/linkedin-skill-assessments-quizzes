## Rust (Programming Language)

#### Q1. Which type cast preserves the mathematical value in all cases?

- [ ] i64 as i32
- [ ] usize as u64
- [x] i32 as i64
- [ ] f64 as f32

#### Q2. What do the vertical bars represent here?

```rust
str::thread::spawn(|| {
    println!("LinkedIn");
});
```

- [x] a closure
- [ ] a thread
- [ ] a future
- [ ] a block

[reference](https://doc.rust-lang.org/book/ch13-01-closures.html#refactoring-with-closures-to-store-code)

#### Q3. Which choice is not a scalar data type?

- [ ] integer
- [ ] float
- [ ] boolean
- [x] tuple

#### Q4. **\_** cannot be destructured.

- [x] Traits
- [ ] Tuples
- [ ] Enums
- [ ] Structs

[reference](https://rust-lang.github.io/rfcs/2909-destructuring-assignment.html)

#### Q5. Which `cargo` command checks a program for error without creating a binary executable?

- [ ] cargo --version
- [ ] cargo init
- [ ] cargo build
- [x] cargo check

#### Q6. The term _box_ and related phrases such as _boxing a value_ are often used when relating to memory layout. What does _box_ refer to?

- [ ] It's creating a pointer on the heap that points to a value on the stack.
- [x] It's creating a pointer on the stack that points to a value on the heap.
- [ ] It's creating a memory guard around values to prevent illegal access.
- [ ] It's an abstraction that refers to ownership. "Boxed" values are clearly labelled.

#### Q7. What is an alternative way of writing `slice` that produces the same result?

```rust
...
let s = String::form("hello");
let slice = &s[0..2];
```

- [ ] let slice = &s[len + 2];
- [ ] let slice = &s[len - 2];
- [ ] let slice = &s.copy(0..2);
- [x] let slice = &s[..2];

#### Q8. Using the `?` operator at the end of an expression is equivalent to **\_**.

- [ ] a match pattern that branches into True or False
- [ ] calling ok_error()
- [ ] calling panic!()
- [x] a match pattern that may result an early return

#### Q9. Which is valid syntax for defining an array of i32 values?

- [ ] Array<i32>::with_capacity(10)
- [ ] [i32]
- [ ] Array<i32>::new(10)
- [x] [i32; 10]

#### Q10. What syntax is required to take a mutable reference to T, when used within a function argument?

```rust
fn increment(i: T) {
    // body elided
}
```

- [ ] \*mut T
- [ ] mut ref T
- [ ] mut &T
- [x] &mut T

#### Q11. The smart pointers Rc and Arc provide reference counting. What is the API for incrementing a reference count?

- [ ] .add()
- [ ] .incr()
- [x] .clone()
- [ ] .increment()

[reference](https://doc.rust-lang.org/book/ch15-04-rc.html)

#### Q12. What happens when an error occurs that is being handled by the question mark (?) operator?

- [ ] The error is reported and execution continues.
- [ ] An exception is raised. The effect(s) of the exception are defined by the error! macro.
- [ ] The program panics immediately.
- [x] Rust attempts to convert the error to the local function's error type and return it as Result::Err. If that fails, the program panics.

#### Q13. Which comment syntax is not legal?

- [ ] `/*`
- [x] `#`
- [ ] `//!`
- [ ] `//`

#### Q14. In matching patterns, values are ignored with \_.

- [ ] `.ignore()`
- [ ] `an underscore (_)`
- [x] ..
- [ ] skip

#### Q15. Defining a \_ requires a lifetime parameter.

- [ ] function that ends the lifetime of one of its arguments
- [x] struct that contains a reference to a value
- [ ] function with a generic argument
- [ ] struct that contains a reference to a boxed value

[Rust book reference](https://doc.rust-lang.org/book/ch10-03-lifetime-syntax.html#lifetime-annotations-in-struct-definitions)

#### Q16. Which example correctly uses std::collections::HashMap's Entry API to populate counts?

```rust
use std::collections::HashMap;
fn main() {
    let mut counts = HashMap::new();
    let text = "LinkedIn Learning";
    for c in text.chars() {
        // Complete this block
    }
    println!("{:?}", counts);
}
```

- [ ]

```rust
for c in text.chars() {
    if let Some(count) = &mut counts.get(&c) {
        counts.insert(c, *count + 1);
    } else {
        counts.insert(c, 1);
    };
}
```

- [x]

```rust
for c in text.chars() {
    let count = counts.entry(c).or_insert(0);
    *count += 1;
}
```

- [ ]

```rust
for c in text.chars() {
    let count = counts.entry(c);
    *count += 1;
}
```

- [ ]

```rust
for c in text.chars() {
    counts.entry(c).or_insert(0).map(|x| x + 1);
}
```

[reference](https://doc.rust-lang.org/std/collections/hash_map/struct.HashMap.html#method.entry)

#### Q17. Which fragment does not incur memory allocations while writing to a "file" (represented by a Vec<u8>)?

```rust
use std::collections::HashMap;

fn main() -> Result<(), Box<dyn std::error::Error>> {
    let mut v = Vec::<u8>::new();

    let a = "LinkedIn";
    let b = 123;
    let c = '🧀';

    // replace this line

    println!("{:?}", v);

    Ok(())
}
```

- [x] :

```rust
write!(&mut v, "{}{}{}", a, b, c)?;
```

- [ ] :

```rust
v.write(a)?;
v.write(b)?;
v.write(c)?;
```

- [ ] :

```rust
v.write(a, b, c)?;
```

- [ ] :

```rust
v.write_all(a.as_bytes())?;
v.write_all(&b.to_string().as_bytes())?;
c.encode_utf8(&mut v);
```

1. [Answered in rust user forum](https://users.rust-lang.org/t/formatting-and-writing-to-a-file-without-malloc-or-locks/52295/9)
2. [reference](https://doc.rust-lang.org/std/macro.write.html)

#### Q18. Does the `main` function compile? If so, why? If not, what do you need to change?

```rust
fn main() {
    let Some(x) = some_option_value;
}
```

- [ ] The code does not compile. `let` statements require a refutable pattern. Add `if` before `let`.
- [ ] The code compiles. `let` statements sometimes require a refutable pattern.
- [x] The code does not compile. `let` statements requires an irrefutable pattern. Add `if` before `let`.
- [ ] The code compiles. `let` do not require a refutable pattern.

#### Q19. Which statement about lifetimes is false?

- [ ] Lifetimes were redundantly specified in previous version of Rust.
- [ ] Lifetimes are specified when a struct is holding a reference to a value.
- [ ] Lifetimes are specified when certain values must outlive others.
- [x] Lifetimes are always inferred by the compiler.

#### Q20. When used as a return type, which Rust type plays a similar role to Python's `None`, JavaScript's `null`, or the `void` type in C/C++?

- [ ] `!`
- [ ] `None`
- [ ] `Null`
- [x] `()`

#### Q21. To convert a `Result` to an `Option`, which method should you use?

- [ ] `.as_option()`
- [x] `.ok()`
- [ ] `.to_option()`
- [ ] `.into()`

#### Q22. Which statement about the `Clone` and `Copy` traits is false?

- [x] `Copy` is enabled for primitive, built-in types.
- [ ] Without `Copy`, Rust applies move semantics to a type's access.
- [ ] When using `Clone`, copying data is explicit.
- [ ] Until a type implements either `Copy` or `Clone`, its internal data cannot be copied.

[ref from stack overflow](https://stackoverflow.com/questions/41413336/do-all-primitive-types-implement-the-copy-trait)

#### Q23. Why does this code _not_ compile?

```rust
fn returns_closure() -> dyn Fn(i32) -> i32 {
    |x| x + 1
}
```

- [ ] The returned `fn` pointer and value need to be represented by another trait.
- [ ] Closures are types, so they cannot be returned directly from a function.
- [ ] Closures are types and can be returned only if the concrete trait is implemented.
- [x] Closures are represented by traits, so they cannot be a return type.

[Rust book reference](https://doc.rust-lang.org/book/ch19-05-advanced-functions-and-closures.html#returning-closures)

#### Q24. What smart pointer is used to allow multiple ownership of a value in various threads?

- [x] `Arc<T>`
- [ ] `Box<T>`
- [ ] Both `Arc<T>` and `Rc<T>` are multithread safe.
- [ ] `Rc<T>`

[Rust book reference](https://doc.rust-lang.org/book/ch16-03-shared-state.html?highlight=arc%3CT%3E#atomic-reference-counting-with-arct)

#### Q25. Which types are _not_ allowed within an enum variant's body?

- [ ] zero-sized types
- [ ] structs
- [x] trait objects
- [ ] floating-point numbers

[Reference](https://doc.rust-lang.org/reference/types/trait-object.html)

#### Q26. Which statement about this code is true?

```rust
fn main() {
    let c = 'z';
    let heart_eyed_cat = '😻';
}
```

- [x] Both are character literals.
- [ ] `heart_eyed_cat` is an invalid expression.
- [ ] `c` is a string literal and `heart_eyed_cat` is a character literal.
- [ ] Both are string literals.

[Reference](https://doc.rust-lang.org/std/primitive.char.html)

#### Q27. Your application requires a single copy of some data type T to be held in memory that can be accessed by multiple threads. What is the thread-safe wrapper type?

- [ ] `Mutex<Arc<T>>`
- [ ] `Rc<Mutex<T>>`
- [x] `Arc<Mutex<T>>`
- [ ] `Mutex<Rc<T>>`

[Rust book reference](https://doc.rust-lang.org/book/ch16-03-shared-state.html#atomic-reference-counting-with-arct)

#### Q28. Which idiom can be used to concatenate the strings `a`, `b`, `c`?

```rust
let a = "a".to_string();
let b = "b".to_string();
let c = "c".to_string();
```

- [ ] `String::from(a,b,c)`
- [x] `format!("{}{}{}", a, b, c)`
- [ ] `concat(a,b,c)`
- [ ] `a + b + c`

#### Q29. In this function. what level of access is provided to the variable `a`?

```rust
use std::fmt::Debug;

fn report<T:Debug>(a: &T) {
    eprintln!("info: {:?}", a);
}
```

- [ ] print
- [x] read-only
- [ ] read/write
- [ ] debug

#### Q30. Which choice is _not_ valid loop syntax?

- [ ] `loop`
- [ ] `for`
- [ ] `while`
- [x] `do`

#### Q31. How do you construct a value of `Status` that is initialized to `Waiting`?

```rust
enum Status {
    Waiting,
    Busy,
    Error(String),
}
```

- [ ] `let s = Enum::new(Status::Waiting);`
- [ ] `let s = new Status::Waiting;`
- [x] `let s = Status::Waiting;`
- [ ] `let s = Status::new(Waiting);`

#### Q32. Which statement about enums is false?

- [ ] Enums are useful in matching patterns.
- [ ] Option is an enum type.
- [ ] Enum variants can have different types with associated data.
- [x] the term _enum_ is short for _enummap_

#### Q33. What does an underscore (\_) indicate when used as pattern?

- [x] It matches everything.
- [ ] It matches underscores.
- [ ] It matches any value that has a length of 1.
- [ ] It matches nothing.

#### Q34. What is a safe operation on a `std::cell:UnsafeCell<T>`?

- [ ] A `&mut T` reference is allowed. However it may not cpexists with any other references. and may be created only in single-threaded code.
- [ ] `UnsafeCell<T>` provides thread-safety. Therefore, creating `&T` references from multiple threads is safe.
- [x] The only safe operation is the `.get()` method, which returns only a raw pointer.
- [ ] Non. `UnsafeCell<T>` only allows code that would otherwise need unsafe blocks to be written in safe code.

[Reference](https://doc.rust-lang.org/stable/std/cell/struct.UnsafeCell.html)

#### Q35. Generics are useful when you **\_**.

- [ ] need to reduce code duplication by concretizing values and restricting parameters in functions
- [x] need to reduce code duplication by abstracting values further, such as in function parameters
- [ ] need a supertrait
- [ ] are not sure if you need a specific kind of trait

#### Q36. How do you create a Rust project on the command-line?

- [x] cargo new
- [ ] rustup init
- [ ] cargo start
- [ ] rust new-project

#### Q37. Calling.clone() **\_**.

- [ ] deeply copies heap data and clones ownership
- [x] clones the pointer to the heap
- [ ] clones the heap data onto the stack
- [ ] deeply copies heap and stack

[Reference](https://doc.rust-lang.org/std/rc/)

#### Q38. what is one of the roles of the let keyword?

```rust
let text = String::new("LinkedIn");
```

- [ ] Create a text object.
- [ ] Assign a mutable value.
- [x] request to borrow a string.
- [ ] Assign an immutable value.

[Reference](https://doc.rust-lang.org/book/ch10-03-lifetime-syntax.html)

#### Q39. How is a new enum initialized?

```rust
enum Option_i32 {
    Some(i32),
    None,
}
```

- [x] let integer = Option_i32::Some(5);
- [ ] let integer = Option_i32.new(Some(5))
- [ ] let integer = Option_i32::New::(Some(5))
- [ ] let integer = Option_i32.init()

[Reference](https://doc.rust-lang.org/rust-by-example/custom_types/enum.html)

#### Q40. What are the main difference between const and static?

- [ ] They can be used interchangeably, but const only supports primitive types while static must be used for structs and user-defined types.
- [ ] They can be used interchangeably, but const values are compiled at compile time.
- [ ] Values defined with const live in the stack, while static values live on the heap.
- [x] Values defined with const can be copied to wherever they are needed, whereas static values remain in a fixed place in memory.

[Reference](https://stackoverflow.com/questions/52751597/what-is-the-difference-between-a-constant-and-a-static-variable-and-which-should)

#### Q41. Which Rust data type represents a signed integer that has the same width as a pointer of the compile target's CPU?

- [ ] i64
- [ ] int64
- [x] isize
- [ ] int

[Reference](https://www.lurklurk.org/effective-rust/use-types.html)

#### Q42. When are supertraits needed?

- [ ] when a trait is needed for multiple structs
- [x] when a trait depends on another trait
- [ ] only when a generic trait is used
- [ ] when a metatrait is needed to use another trait

[Reference](https://doc.rust-lang.org/rust-by-example/trait/supertraits.html)

#### Q43. Which types are legal for x to be in this snippet?

```rust
if x {
    println!("ok");
}
```

- [ ] every type that implements the std::cmp::Truth trait
- [x] only the primitive bool type
- [ ] both bool and u8 (which is how bool is implemented under the hood)
- [ ] bool and std::sync::atomic::AtomicBool

[Reference](https://doc.rust-lang.org/book/ch03-05-control-flow.html#if-expressions)

#### Q44. How do you access the married data in this struct?

```rust
struct person = Person {
    height: u64,
    weight: u64,
    married: bool
}
```

- [ ] person.getMarried()
- [ ] person[married]
- [ ] person.value(married)
- [x] person.married

[Reference](https://doc.rust-lang.org/book/ch05-01-defining-structs.html#accessing-fields-of-a-struct)

#### Q45. To mark a function as visible to other crates, what do you need to do to its definition?

- [ ] Add the public keyword.
- [x] Add the pub keywork.
- [ ] Begin the function's name with a capital letter.
- [ ] Remove the private keyword.

[Reference](https://doc.rust-lang.org/reference/visibility-and-privacy.html)

#### Q46. Which choice is a compound data type?

- [ ] char
- [x] tuple
- [ ] bool
- [ ] i32

[Reference](https://doc.rust-lang.org/book/ch03-02-data-types.html#compound-types)

#### Q47. How could you make this function compile?

```rust
fn main() {
    let x = 5;
    println!("The value of x is: {}", x);
    x = 6;
    println!("The value of x is: {}", x);
}
```

- [ ] Use x only once in a println!() statement.
- [ ] Place curly brackets around let x = 5.
- [ ] Add const to let x = 6.
- [x] Add mut to let x = 5.

[Reference](https://doc.rust-lang.org/book/ch03-01-variables-and-mutability.html)

#### Q48. Using .unwrap() will \_.

- [ ] let you choose the expected panic error message
- [x] call panic! if there is an error or absence of value
- [ ] unwrap the value inside an unsafe wrapper
- [ ] return the error inside Ok()

[Reference](https://doc.rust-lang.org/std/result/enum.Result.html#method.unwrap)

#### Q49. When should the panic! macro be called instead of using std::result::Result?

- [ ] when there is a way to encode the information in types used
- [ ] when your code is expected to end in a good state
- [x] when the situation is considered unrecoverable
- [ ] when valid values are passed on the code

[Reference](https://doc.rust-lang.org/book/ch09-00-error-handling.html)

#### Q50. Which statement about arrays is true?

- [x] [<T>; size of array] can initialize arrays.
- [ ] Indexing, such as array.0, accesses elements in arrays.
- [ ] A data structure for collections can contain different types of values.
- [ ] Arrays are useful when you want to allocate data on the heap and then on the stack.

[Reference](https://doc.rust-lang.org/stable/rust-by-example/primitives/array.html)

#### Q51. How would you select the value 2.0 from this tuple?

```rust
let pt = Point2D(-1.0, 2.0)
```

- [ ] pt[1]
- [ ] pt(1)
- [ ] pt.iter().nth(1)
- [x] pt.1

[Reference](https://doc.rust-lang.org/rust-by-example/primitives/tuples.html)

#### Q52. When writing tests, which macro should you use to assert equality between two values?

- [x] assert_eq!()
- [ ] assert_equal!()
- [ ] is_equals!()
- [ ] assert!()

[Reference](https://doc.rust-lang.org/std/macro.assert_eq.html)
