#PHP Syntax Guide
## PHP is a server-side language sent to the web browser.

## Guide on PHP Basic with examples.
> Including:
-  Comments
-  Variables
-  Echo/Print
-  Data Types
-  Strings
-  Numbers
-  Constants
-  Operators
-  IF & ELSE/ ELSEIF
-  Functions
-  Arrays
-  Loops

**Comments**
```
<?php 
//comments are represented like this or #
//opening php script tag
//closing php script tag
?>
```
**Variables**
> PHP variables are declared with a $ then the name of the variable

``<?php
$pet = "dog";
$PET = "cat";
?>``

> Variables are case-sensitive & will read $pet $PET as different variables
Variables start with a letter or underscore, but cannot start with a number &only contain alpha-numeric characters.

**Strings**
> PHP Strings are a data type and look like this:

```
<?php
$pet2 = "fish";
$_weight = 5.2;

//statements end with ';'
//letters are wrapped in " 
//numbers are not

?>
```
strlen() returns the length of a string
str_word_count() counts the words in a string

**PHP Echo/Print**
> Basic ways to get output. 

```
<?php

echo "Hello World!";
echo () "Hello!";
echo $pet;
//echo can be used () or without
echo "my favourite pet is". $pet . <br>;
// returns: my favourite pet is dog

?>
```

Print can be used that same way: print or print()
```
<?php
print "Hello!";
print() "Hi there!";
print $PET;

?>
```

**Data Types**
PHP includes: 
- String
- Integer
- Float
- Boolean
- Array
- Object
- NULL 

PHP var_dump() returns the value and data type.

```
<?php
//strings
$pet = "dog";
echo $pet;

//integer
non-decimal number, can be negative or positive
$integer = 276;
var_dump($integer);

//Float
A decimal number or exponential
$float = 90.32
var_dump($float);

//Boolean
Boolean is a true or false statement
$_one = true;
$_two = false;

//Array
Arrays holds different values in a one variable.
Declared with array(value);
$pet = array("dog", "cat", "fish");

//Classes + Object
Similar to an array, Objects can contain different values in a single variable.
Classes are templates for objects: has the defined data that the object uses (instance)

class Pet {
  public $species;
  public $coat;
  //public refers to any class can refer to field or method called
  function _construct($species, $coat){
      $this-> = $species;
      $this-> = $coat;
      
     echo "My pet is a" . $this->species . <br> . $this->coat;
     }
  }
  //Object
  $myPet = new Pet("cat", "black");
  
  
  //NULL
  NULL is a datatype that is a variable with no value. Variables can be 'emptied'
  with NULL
  $_null = "Hi!";
  $_null = null;
  var_dump($_null);
  
  ?>
  ```
**Numbers**  
> PHP Numbers include infinity, NaN -integers, and float which are exampled above.
Infinity is a number value larger than `php_float_max`. This can be checked by the functions 
```
- is_finite()
- is_infinite
```
NAN stands for Not a Number, used for operations that aren't possible
```
is_nan()
```
function checks if the value is not a number.

**IF & ELSE & ELSEIF**
> 
  
