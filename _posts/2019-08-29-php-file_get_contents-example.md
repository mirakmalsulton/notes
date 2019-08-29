---
title: PHP - file_get_contents example
---

<h1 class="header">PHP - file_get_contents example</h1>


Example 1
```php
$content = file_get_contents('http://www.google.com/');
echo $content;
// output
// content of url
```


Example 2
```php
$content = file_get_contents('/path/to/file.txt');
echo $content;
// output
// content of file
```