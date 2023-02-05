# ALL YOU NEED TO KNOW || JAVASCRIPT 
## Console
Console is a built-in object that containe error messages or log data and help us to debug our codes.

### console.log();
console.log() is a method that print our output in a message to the browser's developer console.

``` javascript
console.log("Hello, world!");
```

### Variables
Variables, its like a container that used to store and manipulate data in a program.

let and const are the two new keywords that were introduced in ECMAScript 6. The let keyword is used to declare a block-scoped variable, and the const keyword is used to declare a variable that cannot be reassigned.

In JavaScript, variables can be used to hold any type of data like numbers, strings, objects, arrays and functions.

```javascript
let number = 10;
let string = 'Hello World';
let obj = {name: 'John', age: 25};
let array = [1,2,3,4,5];
let func = function(){console.log('Hello')}

```
### Reserved Words
In JavaScript, a reserved word is a word that has a specific meaning and cannot be used as an identifier (such as a variable or function name) in the code. Examples of reserved words in JavaScript include "var", "function", "if", "else", "for", "while", and "return". These words are reserved by the language and cannot be used for any other purpose.

### Data Types
There are two major data type present in JavaScript with sub categories

1. Primitive
    - Number
    - String
    - Boolean
    - Null
    - Undefined
2. Object
    - Array
    - Object
    - Function

### String
 A string is a sequence of characters enclosed in single or double quotes

 ``` javascript
let str = 'String';
let str2 = "String";
let str3 = `String`;
let str4 = String(450);
````

### Boolean 
A Boolean data type is a primitive data type that can have only two values: true or false. Boolean values are often used in conditional statements to check if a certain condition is true or false. For example, you might use a Boolean variable to check if a user is logged in or not.

In JavaScript, you can create a Boolean variable by assigning the values true or false to it, or by using the Boolean() function to convert a non-Boolean value to a Boolean value.

``` javascript
let x = true;
let y = false;
let z = Boolean(1); // true
```

Boolean values are also used in logical operations such as && (and), || (or) and ! (not)

``` javascript
let a = true;
let b = false;
console.log(a && b); //false
console.log(a || b); // true
console.log(!a); // false
```

### Null & Undefined
Null refers to an already assigned value whereas Undefined is a declared variable but its value does not assign yet

``` javascript
    let studentObj = null; //Null
    let studentID; //Undefined
    console.log(studentObj);
    console.log(studentID);
```

### Type Conversion
Type conversion is the process of converting a value from one data type to another data type. For example, converting an integer to a string, or a float to an integer, etc. This is typically done to make sure that data is compatible for certain operations or to match the data type of other values in the same context.

```javascript
// String to Number and Number to String type conversion
let strNumber = "123";
let number = 20;

console.log(strNumber); //string
console.log(number); //number
console.log(Number(strNumber)); // convert a string from string to number
console.log(number.toString()); //convert a number from number to
console.log(String(number)); //convert a number from number to

//Integer to Floating and Floating to Integeer type conversion
let intNumber = 20;
console.log(intNumber);
console.log(typeof parseFloat(intNumber));

let floatNumber = 29.66;
console.log(floatNumber);
console.log(parseInt(floatNumber));
````
### Falsy Value 

```javascripy
false
0 (zero)
"" (empty string)
null
undefined
NaN (Not-a-Number)
```

### Operators 
Operators are symbols that perform specific operations on one or more operands (values or variables) to produce a result. In programming, they are used to manipulate data and variables, compare values, and control the flow of a program. Some common examples of operators include mathematical operators (+, -, *, /), comparison operators (>, <, >=, <=, ==, !=), and logical operators (&&, ||, !).


#### Arithmetic operator (+ - * / % ++ --)
Arithmetic operators are a type of operator used to perform mathematical operations such as addition, subtraction, multiplication, division, and modulus (finding the remainder). These operators are used to perform basic arithmetic calculations on numeric values (integers or floating-point numbers) and are a fundamental part of most programming languages. Examples of arithmetic operators in many programming languages include: 
1. + (addition), 
2. - (subtraction), 
3. * (multiplication), 
4. / (division), and 
5. % (modulus)

```javascript
// Arithmetic Operators

// 1. Addition(+)
let firstNumber = 20;
let secondNumber = 30;
console.log(firstNumber + secondNumber); // + is a Addition sign

// 2. Subtraction(-)
let firstNumber = 20;
let secondNumber = 30;
console.log(firstNumber - secondNumber); // + is a Subtraction sign

// 3. Multiplication(*)
let firstNumber = 20;
let secondNumber = 30;
console.log(firstNumber * secondNumber); // + is a Multiplication 

// 4. Division(/)
let firstNumber = 20;
let secondNumber = 30;
console.log(firstNumber / secondNumber); // + is a Division sign

// 5. Modulus(%)
let firstNumber = 20;
let secondNumber = 30;
console.log(firstNumber % secondNumber); // + is a Modulus sign

// Incremental(++)

// Pre-Incremental
let preIncNumber = 20;
console.log(++incNumber);

//Post-Incremental
let postIncNumber = 20;
console.log(incNumber++);

// Decremental(--)

// Pre-Decremental
let preDecNumber = 20;
console.log(--incNumber);

//Post-Decremental
let postDecNumber = 20;
console.log(incNumber--);

```
### Assignment Operator
An assignment operator is a type of operator that is used to assign a value to a variable in a programming language. The basic syntax of an assignment operator is typically variable = value, where variable is the name of the variable being assigned, and value is the value being assigned to the variable. The assignment operator takes the value on the right side of the operator and stores it in the variable on the left side. For example, the statement x = 10 would assign the value 10 to the variable x. The value of the expression on the right side of the assignment operator is calculated first, and then stored in the variable on the left side.


```javascript
// Assignment Operators
// = += -= *= /= %=
 let a = 30;
 let b = 40;

 a += b // a = a + b

 a -= b // a = a - b

 a *= b // a = a * b

 a /= b // a = a / b

 a %= b // a = a % b
```

### Comparison Operator
A comparison operator is a symbol or operator used to compare values and determine if one value is greater than, less than, equal to, or not equal to another value. These operators return a boolean value (True or False) based on the comparison made between the values. Common comparison operators in programming languages include: >, <, >=, <=, ==, !=, ===, !==

```javascript
// Comparison Operator
// (>, <, >=, <=, ==, !=, ===, !==)

 let a = 20;
 let b = 30;

 console.log(a == b); // false
 console.log(a != b); // true
 console.log(a > b); // false
 console.log(a < b); // true
 console.log(a <= b); // true
 console.log(a >= b); // false

 let a = '50';
 let b = 50;
 console.log(a === b); //false
 console.log(a !== b); // true
```

### Some Math library Uses in JS

```javascript
console.log(Math.E);
console.log(Math.PI);

let n = 4.67;

console.log(Math.abs(n));
console.log(Math.floor(n));
console.log(Math.ceil(n));
console.log(Math.round(n));
console.log(Math.max(345, 100, 765));
console.log(Math.min(345, 100, 765));
console.log(Math.pow(2, 3));
console.log(Math.sqrt(9));
console.log(Math.round(Math.random() * 20 + 1));

```

### Date object in Js

```javascript
let date = new Date();
console.log(date.toDateString());
console.log(date.toLocaleString());
console.log(date.toString());

console.log(date.getFullYear());
console.log(date.getMonth());
console.log(date.getDay());
console.log(date.getDate());
console.log(date.getHours());
console.log(date.getMinutes());
```

### Condition
Conditions in JavaScript allow you to control the flow of your code based on whether certain conditions are met. You can use conditional statements to execute different blocks of code depending on whether a certain condition is true or false.

The most commonly used conditional statements in JavaScript are if, if-else, and switch.

```javascript
let age = 30;

if (age >= 18) {
  console.log("You are an adult.");
}
```





