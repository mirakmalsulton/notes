---
title: PHP - exec example
---

<h1 class="header">PHP - exec example</h1>

```php
exec('ls', $out);
var_dump($out);
// output
// Array
// (
//     [0] => file_1.txt
//     [1] => file_2.txt
//     [2] => file_3.txt
// )
```


```php
exec('whoami', $out);
print_r($out);
// output
// Array
// (
//     [0] => root
// )
```


```php
exec('pwd', $out);
print_r($out);
// output
// Array
// (
//     [0] => /current/working/directory
// )
```