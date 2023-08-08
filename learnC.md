# Learn C
 #  what is C?
 * C is is genreal purpose programming language, created by dennis retchie in 1972.
 * developed in UNIX.
#  why learn C?
* Very popular programming language.
* if you know C, then learning langs like java, c++, python, will be easy for you.
* you can wrtie softwares, games and databases with C.
* Let's create out first C program:
  
  ```sql
  #include <stdio.h>

  int main() {
  printf("Hello World!");
  return 0;
  }
  ```
# C Syntax
* Now lets breakdown the code that we wrote earlier and try to understand it line by line.
* Line 1: ```#include <stdio.h>``` is a header file library, that lets us work out input and output funcations, suck as printf().
* lINE 2: ```main()``` it is function. any code inside curly brackets ```{}``` is going to be executed.
* ```NOTE```: every C statement ends with a semicolon ```;```
* Line 3: ```printf()``` is a funcation used to output the text on the screen.
* line 4: ```return 0``` ends the ```main()``` function.
  # C comments
 * comments are used to explain the code, it can also be used to prevent the execution of some code.
   
* ```single line comments``` (```//```) any text between these two line will be ignored by the compiler.
```sql
 // This is a comment
 printf("hello world");
```
# C Varibales
* Variable is used to store data values, like number and characters.
* in C, there are different types of variable for different keywords, for example:
* ```int``` - stores integers(whole numbers), without decimals, such as ```22```.
* ```float``` - stores floating point number, with decimals, suck as ```20.78```.
* ```char``` - stores single line characters, such as ```'a'``` or ```'b'```, char values are surrounded by single quotes.
  # Declaring variables
* syntax
  
* ```sql
  type variablename = value;
  ```
* in this, *type* is (such as ```int```), and the variablename is the varibale, the equal sign is to assign a value to the variable.
* here is an example:
  
```sql
  int myNum = 15;
```
# Format specifiers
* used together with the ```printf()``` function to tell the compiler what type of data the varibale is storing.
* format specifier always start with ```%```.
* for ```int``` is formart specifier is ```%d``` or ```%i```. ```%c``` for ```char``` and ```%f``` for ```float```.
* Here is an example:
  
 ```sql
  // Create variables
  int myNum = 15;            // Integer (whole number)
  float myFloatNum = 5.99;   // Floating point number
  char myLetter = 'D';       // Character

  // Print variables
  printf("%d\n", myNum);
  printf("%f\n", myFloatNum);
  printf("%c\n", myLetter);
```
* here is one more example:
  
```sql
int myNum = 15;
char myLetter = 'D';
printf("My number is %d and my letter is %c", myNum, myLetter);
```
# change variable values
* you can change the values of variable to another.
* here is an example:
  
  ```sql
  int myNum = 15;

  int myOtherNum = 23;

  // Assign the value of myOtherNum (23) to myNum
  myNum = myOtherNum;

  // myNum is now 23, instead of 15
  printf("%d", myNum);
  ```
# Add variables together
* to add a varibale to another variable, you can use the ```+``` operator.
  
  ```sql
    int x = 5;
  int y = 6;
  int sum = x + y;
  printf("%d", sum);
  ```
  # declare multiple variable
  * you can declare multiple variable of the same type, use the comma.

 ```sql
int x = 5, y = 5, z = 5;
printf("%d", x + y + z);
 ```

    


  
