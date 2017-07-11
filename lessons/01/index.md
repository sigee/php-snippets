"The code is assignment statements, if statements and while loops." - Uncle Bob

## Lesson 01
### Variables
Variables are containers, those can contain data. The data can be different type. In PHP, a variable starts with the $ sign, followed by the name of the variable:

Rules for PHP variables:
- A variable starts with the $ sign, followed by the name of the variable
- A variable name must start with a letter or the underscore character
- A variable name cannot start with a number
- A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )
- Variable names are case-sensitive ($age and $AGE are two different variables)
### Type
#### NULL
Null is a special data type which can have only one value: NULL.
A variable of data type NULL is a variable that has no value assigned to it.
If a variable is created without a value, it is automatically assigned a value of NULL.
#### Array
An array stores multiple values in one single variable.

Example
```php
$cars = array("Volvo","BMW","Toyota");
```
#### Boolean
A Boolean represents two possible states: TRUE or FALSE.

Example
```php
$x = true;
$y = false;
```
#### Float (floating point numbers - also called double)
A float (floating point number) is a number with a decimal point or a number in exponential form.

Example
```php
$x = 3.14;
```
#### Integer
An integer data type is a non-decimal number between -2,147,483,648 and 2,147,483,647.

Rules for integers:
- An integer must have at least one digit
- An integer must not have a decimal point
- An integer can be either positive or negative
- Integers can be specified in three formats: decimal (10-based), hexadecimal (16-based - prefixed with 0x) or octal (8-based - prefixed with 0) or binary (2-based - prefixed with 0b)

Example
```php
$x = 123;
$y = 0x7B;
$z = 0173;
$a = 0b1111011;
```
#### Object
An object is a data type which stores data and information on how to process that data.
In PHP, an object must be explicitly declared.
First we must declare a class of object. For this, we use the class keyword. A class is a structure that can contain properties and methods.

Example
```php
/* PHP 4 */
class Car {
    function Car() {
        $this->model = "VW";
    }
}
$herbie = new Car();
```
```php
/* PHP 5+  */
class Car {
    function __construct() {
        $this->model = "VW";
    }
}
$herbie = new Car();
```
#### Resource
The special resource type is not an actual data type. It is the storing of a reference to functions and resources external to PHP.
A common example of using the resource data type is a database call.
We will not talk about the resource type here, since it is an advanced topic.
#### String
A string is a sequence of characters, like "Hello world!".
A string can be any text inside quotes. You can use single or double quotes.

Example
```php
$x = "Hello world!";
$y = 'Hello world!';
```