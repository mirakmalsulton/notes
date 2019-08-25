---
title: PHP - scandir example
---

<h1 class="header">PHP - scandir example</h1>

Ascending order
```php
$files = scandir('/path/to/dir');
print_r($files);
// output
// Array
// (
//     [0] => .
//     [1] => ..
//     [2] => bar.php
//     [3] => foo.txt
//     [4] => someFolder
// )
```


Descending order
```php
$files = scandir('/path/to/dir', 1);
print_r($files);
// Array
// (
//     [0] => someFolder
//     [1] => foo.txt
//     [2] => bar.php
//     [3] => ..
//     [4] => .
// )
```