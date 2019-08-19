---
title: PHP - fopen example
---

<h1 class="header">PHP - fopen example</h1>

Syntax
```code
fopen(pathToFile, mode);
```

Example
```php
$handle = fopen('/path/to/file.txt', 'r');
while (!feof($file)) {
    $line = fgets($file);
    echo $line;
}
fclose($file);
```