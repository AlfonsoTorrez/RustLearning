## Rust - [1. Getting Started](https://rust-book.cs.brown.edu/ch01-00-getting-started.html)

### Sections
- [1.1 Installation](https://rust-book.cs.brown.edu/ch01-01-installation.html)
	#### Summary 1.1
	- Worked on simple installation of rust. Used Homebrew instead of curl.
- [1.2 Hello, World!](https://rust-book.cs.brown.edu/ch01-02-hello-world.html)
	#### Summary 1.2
	- Created my first Hello World! program. Learned how to run the rust program on my terminal. Used ```println!("text");``` function to output text. 
- [1.3 Hello, Cargo!](https://rust-book.cs.brown.edu/ch01-03-hello-cargo.html)
	#### Summary 1.3
	- Discussed how to use cargo, which is rusts build system/package manager. You can create a new rust program with cargo by using ```cargo new hello_world```, that creates a new directory and project called ```hello_cargo```. Inside you will find a ```.toml``` file and a ```src``` folder (contains rust file). 
	- Filename: ```Cargo.toml```
		```
		[package]
		name = "hello_cargo"
		version = "0.1.0"
		edition = "2021"
		[dependencies]
		```
	- This file is in the ```TOML``` (Tom’s Obvious, Minimal Language) format, which is Cargo’s configuration format. 
	- The first line, [*package*], is a section heading that indicates that the following statements are configuring a package. As we add more information to this file, we’ll add other sections. 
	- The next three lines set the configuration information Cargo needs to compile your program: the name, the version, and the edition of Rust to use. We’ll talk about the edition key in Appendix E. 
	- The last line, [*dependencies*], is the start of a section for you to list any of your project’s dependencies. In Rust, packages of code are referred to as crates. We won’t need any other crates for this project, but we will in the first project in Chapter 2, so we’ll use this dependencies section then.
	- If you started a project that doesn’t use Cargo, as we did with the “Hello, world!” project, you can convert it to a project that does use Cargo. Move the project code into the src directory and create an appropriate Cargo.toml file.


