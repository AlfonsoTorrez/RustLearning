## Chapter 03 - Quiz Questions

1. Which statement best describes what it means if a variable x is immutable?

2. What is the keyword used after let to indicate that a variable can be mutated?

3. Determine whether the program will pass the compiler. If it passes, write the expected output of the program if it were executed. If the program does not pass, indicate the last line number involved in the compiler error.

```
1   fn main() {
2      let x = 1;
3      println!("{x}");
4      x += 1;
5      println!("{x}");
6   }
```

4. Which of the following statements is correct about the difference between using let and const to declare a variable?

5. Determine whether the program will pass the compiler. If it passes, write the expected output of the program if it were executed. If the program does not pass, indicate the last line number involved in the compiler error.

```
const TWO: u32 = 1 + 1;

fn main() {
  println!("{TWO}");
}
```

6. Determine whether the program will pass the compiler. If it passes, write the expected output of the program if it were executed. If the program does not pass, indicate the last line number involved in the compiler error.

```
fn main() {

  let mut x: u32 = 1;

  {
    let mut x = x;
    x += 2;
  }

  println!("{x}");

}
```

7. Determine whether the program will pass the compiler. If it passes, write the expected output of the program if it were executed. If the program does not pass, indicate the last line number involved in the compiler error.

```
fn main() {

  let mut x: u32 = 1;
  x = "Hello world";
  println("{x}");

}
```

8. The largest number representable by the type i128 is:

9. If x : u8 = 0, what will happen when computing x - 1?

10. Determine whether the program will pass the compiler. If it passes, write the expected output of the program if it were executed. If the program does not pass, indicate the last line number involved in the compiler error.

```
fn main() {
  let x: fsize = 2.0;
  println!("{x}");
}
```
