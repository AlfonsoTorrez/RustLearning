## Chapter 03 - Quiz Answers

1. ```x``` cannot be changed after being assigned a value.

2. ```mut```

3. This program does not compile. The last line number in the error is: 4

4. const can be used in the global scope, and let can only be used in a function

5. This program does compile. The output of this program will be: 2

6. This program does compile. The output of this program will be: 1

7. This program does not compile. The last line number in the error is: 3

8. ```2^127 - 1```
    #### Context:
    - In general, a signed number with n bits can represent numbers between -(2^(n - 1)) and 2^(n - 1) - 1.

9. It depends on the compiler mode.
    #### Context:
    - This expression will panic in debug mode and return 255 in release mode.

10. This program does not compile. The last line number in the error is: 
    #### Context:
    - The type fsize does not exist. Floats must be either f32 or f64.

11. This program does compile. The output of this program will be:1
    #### Context:
    - The statement x += 2 only affects the shadowed x inside the inner curly braces, not the outer x on line 2.

12. This program does not compile.
    #### Context:
    - A variable cannot be assigned to a value of a different type than its original type.