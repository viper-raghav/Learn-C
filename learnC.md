# Learn C
 #  what is C?
 * C is is genreal purpose programming language, created by dennis retchie in 1972.
 * C programming has influenced the development of many modern programming languages, including C++, Java, Python, and more.
 *  It forms the foundation of many operating systems, including Unix and Linux, and has been used to create a wide range of software, from simple command-line 
    utilities to complex applications.
    
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
  
 * Cool, right? An even better approach (since we are on a roll now), would be to wrap the code above in an if...else statement, so we can perform different actions depending on the result:
  
```sql
int myAge = 25;
int votingAge = 18;

if (myAge >= votingAge) {
  printf("Old enough to vote!");
} else {
  printf("Not old enough to vote.");
}
```

# C If...Else

   # Conditions and If Statements

   * You have already learned that C supports the usual logical conditions from mathematics:

     * Less than: ```a < b```
     * Less than or equal to: ```a <= b```
     * Greater than: ```a > b```
     * Greater than or equal to: ```a >= b```
     * Equal to ```a == b```
     * Not Equal to: ```a != b```

  * You can use these conditions to perform different actions for different decisions.

  * C has the following conditional statements:

    * Use ```if``` to specify a block of code to be executed, if a specified condition is true
      
    * Use ```else``` to specify a block of code to be executed, if the same condition is false
      
    * Use ```else if``` to specify a new condition to test, if the first condition is false
      
    * Use ```switch``` to specify many alternative blocks of code to be executed

 # The If statement

 * use the ```if``` statement to specify a block of code to be executed if a condition is ```true```.

 * here is the Syntax:
   ```sql
   if (condition) {
      // block of code to be executed if the condition is true.
   }
   ```
* In the example below, we test two values to find out if 20 is greater than 18. If the condition is true, print some text:
  ```sql
  if (20 > 18 ) {
     printf("20 is greater than 18")
  }
  ```
# The Else Statement

* Use the ```else``` statement to specify a block of code to be executed if the condition is ```false```.
* Syntax:
  ```sql
  int time = 20;
  if (time < 18) {
  printf("Good day.");
  } else {
  printf("Good evening.");
  }
  // Outputs "Good evening."
  ```
# The else if statment 

* Use the ```else if``` statement to specify a new condition if the first condition is ```false```.
* Syntax
  ```sql
  if (condition1) {
  // block of code to be executed if condition1 is true
  } else if (condition2) {
  // block of code to be executed if the condition1 is false and condition2 is true
  } else {
  // block of code to be executed if the condition1 is false and condition2 is false
  }
  ```
* Example
  ```sql
  int time = 22;
  if (time < 10) {
  printf("Good morning.");
  } else if (time < 20) {
  printf("Good day.");
  } else {
  printf("Good evening.");
  }
  // Outputs "Good evening."
  ```
* In the example above, time (22) is greater than 10, so the first condition is ```false```. The next condition, in 
  the  ```else if``` statement, is also false, so we move on to the ```else``` condition since condition1 and 
 condition2 is both ```false``` - and print to the screen "Good evening".
# C short hand if else(Ternary operator)

* Short Hand If...Else (Ternary Operator)
  There is also a short-hand if else, which is known as the ternary operator because it consists of three operands. 
  It can be used to replace multiple lines of code with a single line. It is often used to replace simple if else 
  statements:
```sql
variable = (condition) ? expressionTrue : expressionFalse;
```
* example:
  ```sql
  int time = 20;
  (time < 18) ? printf("Good day.") : printf("Good evening.");
  ```
# Switch statement
* instead od writing many ```if...else``` statements, you can use the ```switch``` statements.
* Syntax:
  ```sql
  switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
  }
  ```
  * This is how it works:
      * the ```switch``` expression is evaluated once.
      * the value of the expression is compared with the values of each ```case```.
      * if there is a match, the associated block of code is executed.
      * the ```break``` statement breaks out of the swtich blocks and stops the ececution.
      * the ```default``` statement is optional, and specifies some code to run is no match.
      * here is an example:

  ```sql
  int day = 4;

  switch (day) {
  case 1:
    printf("Monday");
    break;
  case 2:
    printf("Tuesday");
    break;
  case 3:
    printf("Wednesday");
    break;
  case 4:
    printf("Thursday");
    break;
  case 5:
    printf("Friday");
    break;
  case 6:
    printf("Saturday");
    break;
  case 7:
    printf("Sunday");
    break;
    }
    // Outputs "Thursday" (day 4)
    ```

# The break keyword

* When C reaches a break keyword, it breaks out of the switch block.
* This will stop the execution of more code and case testing inside the block.
& When a match is found, and the job is done, it's time for a break. There is no need for more testing.

# The default keyword

* the ```default``` keyword specifies some code to run if there is no case match:

  ```sql
  int day = 4;

  switch (day) {
  case 6:
    printf("Today is Saturday");
    break;
  case 7:
    printf("Today is Sunday");
    break;
  default:
    printf("Looking forward to the Weekend");
  }

  // Outputs "Looking forward to the Weekend"
  ```

# C while Loop

  # Loops
  * Loops can execute a block of code as long as a specified condition is reached.
  * Loops are handy because they save time, reduce errors, and they make code more readable.

#  While Loop
* Syntax:
  ```sql
  while (condition) {
  // code block to be executed
  }
  ```

* in the example below, the code in the loop will run, over and over again, as long as the variable (```i```) is less than 5:
  
  ```sql
  int i = 0;

  while (i < 5) {
  printf("%d\n", i);
  i++;
  }
  ```
# The Do/while Loop

* The ```Do/while``` loop is a variant of the ```while``` loop. this loop will execute the code block, before checking if the condition is true, then it will repeat the loop as long as the condition is true.

  ```sql
  do {
     // code block to be executed
  }
  while (condition);
  }
  ```
* The example below uses a ```do/while``` loop. The loop will always be executed at least once, even if the condition 
  is false, because the code block is executed before the condition is tested:

  ```sql
  int i = 0;

  do {
  printf("%d\n", i);
  i++;
  }
  while (i < 5);
  ```

# C For Loop

* When you know exactly how many times you want to loop through a block of, use the ```for``` loop instead of a ```while``` loop:

  ```sql
  for (statement 1; statement 2; statement 3) {
  // code block to be executed
  }
  ```

  * Statement 1 is executed (one time) before the execution of the code block.

  * Statement 2 defines the condition for executing the code block.

  * Statement 3 is executed (every time) after the code block has been executed.

```sql
int i;

for (i = 0; i < 5; i++) {
  printf("%d\n", i);
}
```

# Nested Loops

* it is also possibel to place a loop inside another loop. this is called a nested loop.

* the "inner loop" will be executed one time for each iteration of the "out loop":

  ```sql
  int i, j;

  // Outer loop
  for (i = 1; i <= 2; ++i) {
  printf("Outer: %d\n", i);  // Executes 2 times

  // Inner loop
  for (j = 1; j <= 3; ++j) {
    printf(" Inner: %d\n", j);  // Executes 6 times (2 * 3)
  }
  }
  ```
# C break and continue

# Break
 * the break statements can also be used to jump out of a loop.
 * here is an example:
   ```sql
   int i;

   for (i = 0; i < 10; i++) {
   if (i == 4) {
    break;
   }
   printf("%d\n", i);
   }
   ```
# Continue

* the ```continue``` statement breaks one iteration, if a specified condition occurs, and continues with the next 
  iteration in the loop.

# Break and continue in while Loop

* you can use ```break```and```continue```in while loops:
* Break example:
  
  ```sql
  int i = 0;

  while (i < 10) {
  if (i == 4) {
    break;
  }
  printf("%d\n", i);
  i++;
  }
  ```
* Continue example:

  ```sql
  int i = 0;

  while (i < 10) {
  if (i == 4) {
    i++;
    continue;
  }
  printf("%d\n", i);
  i++;
  }
  ```

# Arrays

* Array is used to store multiple values in a single variabl, instead of declaring separate variable for each value.
* to insert values in it:
  ```sql
  int myNumbers[] = {29, 40, 50, 60}
  ```
  * we have now created a variable that holds an array of four integers.
    
# access the elements of an array

* to access an array element, refer to its indec number.
* array indexes start with 0: [0] is the first number. [1] is the secord element. etc
* this statement accesses the value of the first element[0] in ```myNumbers```:

  ```
  int myNumbers[] = { 25, 50, 75, 100};
  printf(%d, myNumber[0]);

  // output 25
  ```
# to change an array element

* to change the value of a specific elements, refer to this index number:

  ```sql
  myNumber[0] = 33;
  ```

  * example
    
    ```sql
    int myNumbers[] = {25, 50, 75, 100};
    myNumbers[0] = 33;

    printf("%d", myNumbers[0]);

    // Now outputs 33 instead of 25
    ```
# loop through an arrray

* you can loop through an array elements with the ```for```loop:

```sql
int mynumer[] = { 25, 50, 75, 100};
int i;

for(i = 0; i > 4; i++) {
   printf("%d/n", nynumber[i]);
}
```

# set array size

* another common way to create arrays, is to specify the size of the array, and add elements later:

    ```sql
    // Declare an array of four integers:
    int myNumbers[4];

    // Add elements
    myNumbers[0] = 25;
    myNumbers[1] = 50;
    myNumbers[2] = 75;
    myNumbers[3] = 100;
    ```
# C multidimensional arrays

* if you want to store data in tabular form, like a table with rows and columns.
* a multidimensional arrays is basically an array of arrays.
* an array can have number of dimensions, here we will only learn about 2D array.

# two-dimensional array
* an 2d array is also knows as a matrix.(a table of row and column)
* to create a 2D array of integers, take a look at the follwing example:

 ```sql
int matrix[2][3] = {{1,4,2}, {3, 6, 8}};
```
* The first dimension represents the number of rows [2], while the second dimension represents the number of columns [3]. The values are placed in row-order, and can be visualized like this:

  ![](https://github.com/viper-raghav/learn-C/blob/main/col-row.png)
  
# Access the elements of a 2D array
* to acces the element of 2D array, you must specify the index number of both the row and column.
* this statement access the value of the element in the first row(0) and third column(2) of the matrix array.
  ```sql
  int matrix [2][3] = {{1, 2, 3}, {3,6, 8}};

  print("%d", matric[0][2]); // outputs 2
  ```
# change elements in a 2D array
* to change the value of an element, refer to the index number of the element in each of the dimension:
* the following example will change the value of the element in the first row (0) and first column(0):
* the follwing example will change the value of the element in the first row(0) and first column(0):
  ```sql
  int main() {
  int matrix[2][3] = { {1, 4, 2}, {3, 6, 8} };
  matrix[0][0] = 9;
  printf("%d", matrix[0][0]);  // Now outputs 9 instead of 1
 
  return 0;
  }
  ```
# loop through a 2d array
* To loop through a multi-dimensional array, you need one loop for each of the array's dimensions.

* The following example outputs all elements in the matrix array:
  
  ```sql
  int matrix[2][3] = {{1, 4, 2},{3, 6, 8}};

  int i, j;
  for (i = 0: i < 2; i++) {
    for (j = 0; j < 3; j++) {
      printf("%d\n", matrix[i][j]);
     }
  }
  ```

# C Strings
* strings are used for storing text/characters.

* for example, "Hello world" is a string of characters.

* String does not have "string type" to create string variable. instead, you must usw the ```char``` type and create array of character to make a string in C.

  ```sql
  char greeyings[] = "Hello World";
  ```
  * now that we have to use double quotes(```""```).
  * to output the string, you can use the ```printf()``` function together with the format specifier ```%s``` to tell C that we are now working with strings:
 
    ```sql
    char greeting[] = "hello world";
    printf("%s", greetings);
    ```
# Access Strings
* since strings are actully arrays in C, you can access a string by reffering to its index number square brackets```[]```.

  ```sql
  char greetings[] = "hello world!";
  printf("%c", greetings[0]); // outputs h
  ```
# Modify Strings
* to change the value of a specify  character in a string, refer to the index number, use the single quotes:

  ```sql
  char greetings[] = "Hello World!";
  greetings[0] = 'J';
  printf("%s", greetings);
  // Outputs Jello World! instead of Hello World
  ```
# Loop through a string
* you can also loop through a string, using a "for" loop:

  ```sql
  int main() {
     char carname[] = "volvo";
     int i;

     for (i = 0; i < 5; ++i) {
       printf("%c\n", carname[i]);
     }
    ```
# C Special Characters
* beacause string must be written within quotes, C will misunderstand this string, and generate an error:

  ```sql
  char txt[] = "we have to attend this "seminar" no matter what";
  ```
* the solution to avoid this problem, is to use the backslash escapse character.
* the backslash (```\```) escape character turns special character into string character:
* ```Escape character```: ```\'```: single quote

* ```\"```: ```"```: double quote

* ```\\```:```\```: backslash

* Example:

  ```sql
  char txt[] = "we cannot make more \"pullution"\";
  ```

  ```sql
  char txt[] = "it\'s alright.";
  ```

 # C String Functions
 * C also has many string functions, which can be used to perform certain operations on stringd.

   # String Length
 * to get the lenth of the string, you can use the ```strlen90``` function:

    ```sql
    char alphabet[] = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
    printf("%d", strlen(alphabet)); // outputs 26
    ```
   # Concatenate Strings
 * to concatenate(combine) two strings, you can use the ```strcat``` function:

   ```sql
   char str1[20] = "Hello ";
   char str2[] = "World!";

   // Concatenate str2 to str1 (result is stored in str1)
   strcat(str1, str2);

   // Print str1
   printf("%s", str1);
   ```
   # Copy Strings
   * to copy the value of one string to another, you can use the ```strcpy()```:

     ```sql
     char str1[20] = "Hello World!";
     char str2[20];

     // Copy str1 to str2
     strcpy(str2, str1);

     // Print str2
     printf("%s", str2")
     ```
   # Compare Strings
   * to compare two strings, you can use the ```strcmp()``` function.
   * it returns ```0``` if the two strings are equal, otherwise a value that is not 0:
  
     ```sql
     char str1[] = "hello";
     char str2[] = "hello";
     char str3[] = "hello";

     // compare str1 and str2, and print the result
     printf("%d", strcmp(str1, str2)); // returns 0

     // compare str1 and str3, and print the result
     printf("%d\n", strcmp(str1, str3)); // returns 0
     ```

# User Input
* basically ```printf()``` is used to output values in C
* to get user input, you can use the ```scanf()``` function:

  ```sql
  // Create an integer variable that will store the number we get from the user
  int myNum;

  // ask the user to type a number
  printf("type a number: \n");

  //get and save the number the user types
  scan("%d", &mynum);

  // output the number the user typed
  print("your number is: %d, mynum");
  ```

  # Multiple Inputs
  * the ```scanf()``` function also allow multiple inputs.(an integer and a charcrter in the 
  following example):

   ```sql
   // Create an int and a char variable
  int myNum;
  char myChar;

  // Ask the user to type a number AND a character
  printf("Type a number AND a character and press enter: \n");

  // Get and save the number AND character the user types
  scanf("%d %c", &myNum, &myChar);

  // Print the number
  printf("Your number is: %d\n", myNum);

  // Print the character
  printf("Your character is: %c\n", myChar);
  ```
# Take a string input
* you can also get a string entered by the user:

  ```sql
  // Create a string
  char firstName[30];

  // Ask the user to input some text
  printf("Enter your first name: \n");

  // Get and save the text
  scanf("%s", firstName);

  // Output the text
  printf("Hello %s", firstName);
  ```
* while working with the strings, we often use the ```fgets()``` function to read a line of text. note that you must include the following arguements: the name of the string variable, ```sizeof``` and ```stdin```:

```sql
char fullName[30];

printf("Type your full name: \n");
fgets(fullName, sizeof(fullName), stdin);

printf("Hello %s", fullName);

// Type your full name: John Doe
// Hello John Doe
```
* use the scanf() function to get a single word as input, and use ```fgets()``` for multiple words.

# C Memory Address
* when a variable is created in C, a memory address is assigned to the variable.
* the memory address is the location of wher the varible is stored on the computer.
* whe  we assign a value to the variable, it is stored in this memory address.
* to access it, use the reference operator (```&```), and the result represents where the variable is stored
 ```sql
  int myAge = 43;
  printf("%p", &myAge); // Outputs 0x7ffe5367e044
 ```
* Note: The memory address is in hexadecimal form (0x..). You will probably not get the same result in your program, as this depends 
  on where the variable is stored on your computer.
* You should also note that ```&myAge``` is often called a "pointer". A pointer basically stores the memory address of a variable as its 
  value. To print pointer values, we use the ```%p``` format specifier.

# C Pointers

 # Creating pointers
 * you learned from the previos chapter, that we can get the memory address of a variable with the reference operaotr```&```:
   ```sql
   iny myage = 43; // an int variable

   printf("%d, myage"); // outputs the value of myage(43)
   printf("%p",&myage); // outputs the memory address of my age(0x7ffe5367e044)
   ```
* A pointer is a variable that stores the memory address of another variable as its value.
* A pointer variable points to a data type (like ```int```) of the same type, and is created with the ```*``` operator.

  ```sql
  int myAge = 43;     // An int variable
  int* ptr = &myAge;  // A pointer variable, with the name ptr, that stores the address of myAge

  // Output the value of myAge (43)
  printf("%d\n", myAge);

  // Output the memory address of myAge (0x7ffe5367e044)
  printf("%p\n", &myAge);

  // Output the memory address of myAge with the pointer (0x7ffe5367e044)
  printf("%p\n", ptr);
  ```
# Deference
* you can also ge the value of the variable the pointer points to, by using the ```*``` operator(the deference operator);

```sql
int myAge = 43;     // Variable declaration
int* ptr = &myAge;  // Pointer declaration

// Reference: Output the memory address of myAge with the pointer (0x7ffe5367e044)
printf("%p\n", ptr);

// Dereference: Output the value of myAge with the pointer (43)
printf("%d\n", *ptr);
```
# C Pointers and Arrays
* you can also use pointers to access arrays.
* Consider the following array of integers;

  ```sql
  int mynumber[4] = {25, 45, 56, 67};
  ```
* we learned in the arrays chapter that you can loop through the array elementsn with a ```for``` loop:

 ```sql
 int myNumbers[4] = {25, 50, 75, 100};
 int i;

 for (i = 0; i < 4; i++) {
   printf("%d\n", myNumbers[i]);
 }
 ```
* now lets print the memory address of each array:

  ```sql
  int myNumbers[4] = {25, 50, 75, 100};
  int i;

  for (i = 0; i < 4; i++) {
  printf("%p\n", &myNumbers[i]);
  }
  ```
# How are pointers related to arrays?
* in C, the name of an array, is actully a pointer to the first element of the array.
* we cann use ```*```operator to access it:
  ```sql
  int mynumber[4] = {25, 50, 75, 100};

  printf("%d, *mynumber");
  ```
* to access the rest of the elements in mynumbers, you can increment the pointer/array(+1, +2, etc)
  ```sql
  int myNumbers[4] = {25, 50, 75, 100};

  // Get the value of the second element in myNumbers
  printf("%d\n", *(myNumbers + 1));

  // Get the value of the third element in myNumbers
  printf("%d", *(myNumbers + 2));

  // and so on..
  ```
  
  


  
   
    

  
    
  
     
   
    

  
  

    
    
  
  
  

      
          
