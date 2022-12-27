## Code Snippets
- Useful code snippets collected from the Rust book. 
- ```command```* = use on terminal

### Code & Description

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