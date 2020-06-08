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


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/09/01/php-round-up-round-down-example">
                php round up round down example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/09/01/php-round">
                php round
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/29/php-spl_autoload_register-example">
                php spl_autoload_register example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/29/php-strtotime-examples">
                php strtotime examples
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/29/php-file_get_contents-example">
                php file_get_contents example
            </a>
        </li>
    </ul>
</div>