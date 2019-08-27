---
title: PHP - ob_start example
---

<h1 class="header">PHP - ob_start example</h1>

```php
ob_start(); // captures the output and save it in an internal buffer
echo("world!"); // "world!" saved in internal buffer
$output = ob_get_contents(); // save in a variable internal buffer content
ob_end_clean(); // clean internal buffer
echo 'Hello ' . $output;
// output
// Hello world!
```


```php
ob_start();
echo("Hello world!");
$output = ob_get_contents();
ob_end_flush(); // print internal buffer content
// output
// Hello world!
```