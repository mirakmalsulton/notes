---
title: PHP - str_replace example
---

<h1 class="header">PHP - str_replace example</h1>


Syntax
```php
str_replace($find, $replace, $string, $count)
```

Example 1
```php
$string = 'Hello world!';
$find = 'world!';
$replace = 'foo bar!';
$result = str_replace($find, $replace, $string);
echo $result;
// output
// Hello foo bar
```


Example 2
```php
$string = 'Hello world!';
$find = 'o';
$replace = '';
$result = str_replace($find, $replace, $string, $count);
print_r($count);
// output
// 2
```
