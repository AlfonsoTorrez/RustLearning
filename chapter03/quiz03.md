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