---
title: PHP - recursive function example
---

<h1 class="header">PHP - recursive function example</h1>

<div style="color:#555;margin-bottom:30px;">
    A recursive function is a function that calls itself.
</div>

```php
/**
 * Use with care!
 * Recursively delete a file or directory.
 * @param string $path
 */
function recursiveRemove($path)
{
    if (is_dir($path)) {
        foreach (scandir($path) as $entry) {
            if (!in_array($entry, ['.', '..'])) {
                recursiveRemove($path . DIRECTORY_SEPARATOR . $entry); // calls itself
            }
        }
        rmdir($path);
    }
    if (is_file($path)) unlink($path);
}

recursiveRemove('/path/to/dir');
```
