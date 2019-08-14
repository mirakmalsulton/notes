---
title: PHP - get file size
---

<h1 class="header">PHP - get file size</h1>

```php
$file = 'my_file.txt';
echo $file . ': ' . filesize($file) . ' bytes';
//output
//my_file.txt : 10 bytes
```