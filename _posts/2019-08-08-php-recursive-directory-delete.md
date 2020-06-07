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


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/29/php-file_get_contents-example">

            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/29/php-strtotime-examples">

            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/29/php-spl_autoload_register-example">

            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/09/01/php-round">

            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/09/01/php-round-up-round-down-example">

            </a>
        </li>
    </ul>
</div>