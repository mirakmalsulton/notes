---
title: PHP - recursive directory delete
---

<h1 class="header">PHP - recursive directory delete</h1>

```php
function recursiveRmDir($path)
{
    if (is_dir($path)) {
        foreach (scandir($path) as $entry) {
            if (!in_array($entry, ['.', '..'])) {
                recursiveRmDir($path . DIRECTORY_SEPARATOR . $entry);
            }
        }
        rmdir($path);
    }
    if (is_file($path)) unlink($path);
}
recursiveRmDir('/var/www/my_dir');
```