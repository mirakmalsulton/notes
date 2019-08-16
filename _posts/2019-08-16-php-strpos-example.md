---
title: PHP - strpos example
---

<h1 class="header">PHP - strpos example</h1>

Find the position of the first occurrence of a substring in a string
```php
$string = 'hello world';
$post = strpos($string, 'world'); // $pos = 6
$post = strpos($string, 'o'); // $pos = 4
```

ignoring anything before the offset
```php
$post = strpos($string, 'o', 5); // $pos = 7
```