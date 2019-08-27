---
title: PHP - file_put_contents example
---

<h1 class="header">PHP - file_put_contents example</h1>


<div style="color:#555;margin-bottom:30px;">
    <b>file_put_contents</b> writes data to the file.
    The data to write can be either a string, an array or a stream resource
</div>


Example 1
```php
$array = [1, 2, 3];
file_put_contents('file.txt', $array);
//If file.txt doesn't exist, it will be created.
//file.txt content will be "123"
```

Example 2
```php
file_put_contents('file.txt', 'a');
//file.txt content will be "a"

file_put_contents('file.txt', 'b');
//Deletes the existing content of the file. file.txt content will be "b"

file_put_contents('file.txt', 'c', FILE_APPEND);
//FILE_APPEND - avoid deleting the existing content of the file
//file.txt content will be "bc"
```