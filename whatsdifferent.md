What's different in Rust from other languages
=

- In Rust, following is a valid function.
```
fn five () -> u32 {
  5
}
```
It is because the literal `5` is considered an expression. Expressions return values and statements don't. Putting a semi-colon after `5` will make it a statement and that will make the function to throw an error.

## Other relevant tips
- The following creates a copy of variable x (on stack):\
```
let x = 5;
let y = x;
```
  While the following creates a copy of pointer to the string (on stack) and the actual data is on the heap and referenced by both x and y.
```
let x = String::from('hello');
let y = x;
```
