## Code Snippets
- Useful code snippets collected from the Rust book. 
- ```command```* = use on terminal

## Code & Description

```rustup update```*
- Command to update rust version. 

```rustup self uninstall```*
- Command to uninstall rust. 

```rustup doc```*
- Opens the local documentation in your browser.

```println!("Hello World!")```
- Simple output function for printing out basic strings. 

```cargo build```*
- This command creates an executable file in ```target/debug/hello_cargo``` (or ```target\debug\hello_cargo.exe``` on Windows) rather than in your current directory. Because the default build is a debug build, Cargo puts the binary in a directory named debug. 
- Running cargo build for the first time also causes Cargo to create a new file at the top level: ```Cargo.lock```.

```cargo run```*
- We just built a project with cargo build and ran it with ```./target/debug/hello_cargo```, but we can also use ```cargo run``` to compile the code and then run the resulting executable all in one command
- Using ```cargo run``` is more convenient than having to remember to run ```cargo build``` and then use the whole path to the binary, so most developers use ```cargo run```.

```cargo check```*
- This command quickly checks your code to make sure it compiles but doesn’t produce an executable. 

```cargo build --release```*
- Creating a final program to give to another user. 

### Float-Point Types
```
    let x = 2.0; // f64
    let y: f32 = 3.0; // f32
```

### Numeric Operations
```
    // addition
    let sum = 5 + 10;

    // subtraction
    let difference = 95.5 - 4.3;

    // multiplication
    let product = 4 * 30;

    // division
    let quotient = 56.7 / 32.2;
    let floored = 2 / 3; // Results in 0

    // remainder
    let remainder = 43 % 5;
```

### Boolean Type
```
    let t = true;
    let f: bool = false; // with explicit type annotation
```

### Character Type
```
    let c = 'z';
    let z: char = 'ℤ'; // with explicit type annotation
    let heart_eyed_cat = '😻';
```