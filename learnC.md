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
# Type Conversion
* sometimes we have to convert the value of one data type to another type.
  
* for example, if you try to divide two integers, ```5``` by ```2```, you cannot get ```2.5```, but since we are working with integers (not floating integers).
  
* to get *type conversion*, there are two type of conversion in C:
   * Implicit conversion(automatic)
   * xplicit conversion(manually)

# Implicit Conversion
* Done automatically by the compiler, whien you assingn a value of one type to another.
  
  * Example
    
  ```sql
    // Automatic conversion: int to float
    float myFloat = 9;

    printf("%f", myFloat); // 9.000000
  ```
  * one more example

    ```sql
    // Automatic conversion: float to int
    int myInt = 9.99;

    printf("%d", myInt); // 9
    ```
# Explicit Conversion
* it is done manually.
* by placing the type in ```()``` in front of the value.

  ```sql
  // Manual conversion: int to float
  float sum = (float) 5 / 2;

  printf("%f", sum); // 2.50000
  ```
# C Constants
* If you dont want to change the values of the existing variables values, you can use the ```const``` keyword.
* this will declare the the variable as "constant", which means unchangeable or 
 read-only
  
  ```sql
  const int myNum = 15;  // myNum will always be 15
  myNum = 10;  // error: assignment of read-only variable 'myNum'
  ```
# C Operator
* used to perform operations on variables and values.

  ```sql
  int num = 100 + 50;
  ```
  * C divided the operator into follwing groups:

    * Arithmatic operator
    * Assignment operators
    * Comparison operators
    * Logical operators
    * Bitwise operators

# Arithmatic operator
* used to perform mathematical operations.
operator    Name            Description

        ```+```   Addition,        adds two digits together
 
        ```-```   substration ,    substracts one value form another
 
        ```*```    Multiplication , Multiplies two values

        ```/```    Division,        Divides one value by another

        ```%```    modulus,         returns the division remainder

        ```++```   Increment,      Increase the value of a variable by 1

        ```--```   Decrement,       Decreases the value of a variable by 1

# Assignment Operators
* used to assign values to variables. we use (```=```).

  ```sql
  int x = 10;
  ```
  ```sql
  int x = 10;
  x += 5;
  ```
  * here ```+=``` is used to add value to a variable.
    
  * here is the list of Assignment operator:

     * ```=```
    
     * ```+=```

     * ```-=```

     * ```*=```
   
     * ```/=```
   
     * ```%=```
   
     * ```&=```
   
     * ```|=```
   
     * ```^=```
    
     * ```>>=```
   
     * ```<<=```
#  Comparison operator
* used to compare two values.
* The return value of a comparison is either ```1``` or``` 0```, which means true (```1```) or false (```0```). These values are known as Boolean values
  
     ```sql
     int x = 5;
     int y = 3;
     printf("%d", x > y); // returns 1 (true) because 5 is greater than 3
     ```
* list of comparison operators:
     * ```==```
     * ```!=```
     * ```>```
     * ```<```
     * ```>=```
     * ```<=```
 
# Logical Operator
* you can test for true or flase with logical operator.
  ```sql
  ```&&``` LOGICAL AND, Returns true if both statements are true. e.g. x < 5 && x < 
                        10
  
  ```||``` LOGICAL OR, returns true if one of the statements is true. e.g. x <5 || 
                       x < 4
  
  ```!```  LOGICAL NOT, reverse the result, returs false if the result is true.!(x 
                        < 5 && x < 10)
  ```

#Sizeof Operator

* The memory size (in bytes) of a data type or a variable can be found with the sizeof operator:

   ```sql
   int myInt;
   float myFloat;
   double myDouble;
   char myChar;

   printf("%lu\n", sizeof(myInt));
   printf("%lu\n", sizeof(myFloat));
   printf("%lu\n", sizeof(myDouble));
   printf("%lu\n", sizeof(myChar));

   // OutPut
      4
      4
      8
      1
   ```

# Booleans

 * Very often, in programming, you will need a data type that can only have one of two values, like:

     * YES / NO
     * ON / OFF
     * TRUE / FALSE
       
* For this, C has a ```bool``` data type, which is known as booleans.

Booleans represent values that are either ```true``` or ```false```.

* a boolean variable is declared witht he ```bool``` keyword and can only take the value ```true``` or ```false```.

  ```sql
      bool isProgrammingFun = true;
      bool isFishTasty = false;
  ```
  Before trying to print the boolean variable, you should know that boolena values are returned as integers:
     * ```1``` (or any other number that is not 0) represents ```true```
     *  ```0``` represents ```false```
# comparing valus and variables
 * Comparing values are useful in programming, because it helps us to find answers 
   and make decisions.

* For example, you can use a comparison operator, such as the greater than (>) 
  operator, to compare two values:

  ```sql
  printf("%d", 10 > 9);  // Returns 1 (true) because 10 is greater than 9
  ```
  

   
  
   

      
          
