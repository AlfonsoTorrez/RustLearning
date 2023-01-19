## Code Snippets
- Useful code snippets collected from the Rust book. 
- ```command```* = use on terminal

## Code/Vocabulary & Description

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

### Compound Types 
- ```Compound types``` can group multiple values into one type. Rust has two primitive compound types: ```tuples``` and ```arrays```.

### Tuple Type
- A ```tuple``` is a general way of grouping together a number of values with a variety of types into one compound type.

```
    let tup: (i32, f64, u8) = (500, 6.4, 1);
```

### Destructuring
- Using ```let``` to take ```tup``` and turn it into 3 seperate variables. 
```
    let tup: (i32, f64, u8) = (500, 6.4, 1);
    let (x, y, z) = tup;
    println!("The value of y is: {y}");
    //Output: The value of y is: 6.4
```

### Use by Index
```
    let x: (i32, f64, u8) = (500, 6.4, 1);
    let five_hundred = x.0;
    //Output: 500
    let six_point_four = x.1;
    //Output: 6.4
    let one = x.2;
    //Output: 1
```

### Array Type
- An ```Array``` is a variable that can store multiple values. Unlike a tuple, every element of an array must have the same type. Unlike arrays in some other languages, arrays in Rust have a fixed length.
```
fn main() {
    let a = [1, 2, 3, 4, 5];
}
```
- Here, ```i32``` is the type of each element. After the semicolon, the number ```5``` indicates the array contains five elements.
```
fn main() {
    let a: [i32; 5] = [1, 2, 3, 4, 5];
}
```

### Accessing Array Elements
```
fn main() {
    let a = [1, 2, 3, 4, 5];

    let first = a[0];
    let second = a[1];
}
```
- In this example, the variable named ```first``` will get the value ```1```, because that is the value at index [0] in the array. The variable named ```second``` will get the value 2 from index ```[1]``` in the array.