# GumGum Web Engineering - PHP Test
# Snippets

Integers and other numbers
--------------------------
- What will be the output of the following statements:
```php
var_dump(0123 == 123);
var_dump('0123' == 123);
var_dump('0123' === 123);
```
- What will be the value of the variables x and y? Why? How does that works?
```php
$x = 4 && 6;
$y = 8 & 1;
```
- What is PHP_INT_MAX? What is the result on each statement? Why?
```php
var_dump(PHP_INT_MAX+1);
var_dump((int)PHP_INT_MAX+1);
```
- What is a try-catch block?
 - Write an example.
 - How would you use it in a MVC codebase?

Arrays
------
- What will be printed?
```php
$a = array();
if ($a == null) {
    echo 'Indeed.';
} else {
    echo 'Nope.';
}
```
- Besides array_push(), name other ways to add elements to an array.
- What's the difference between [ ] and Array() ?
- What's the maximum allowed items in an array?
- What will be printed?
```php
echo count([
    null => 'a',
    true => 'b',
    false => 'c',
    0 => 'd',
    1 => 'e',
    '' => 'f',
]);
```
- What's SplFixedArray and why does it exist?
- You have an array of random dates of a year, index them by month and order asc:
```php
$days = ['2015-01-01','2015-01-02','2015-02-20','2015-03-24','2015-03-21', ...];
$indexed = theFunction($days);
/*
[
    '01' => ['2015-01-01', '2015-01-02'],
    '02' => ['2015-02-20'],
    '03' => ['2015-03-21','2015-03-24'],
]
*/
```

OOP
---
- What does spl_autoload_register do?
- What is late static binding?
- What is Type hinting and what are its limitations on PHP5?
- Explain in lay terms the concepts of the following terms, and write some use cases:
 - Abstract classes
 - Interfaces
 - Traits
