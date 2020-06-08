---
title: PHP - spl_autoload_register example
---

<h1 class="header">PHP - spl_autoload_register example</h1>

<div style="color:#555;margin-bottom:30px;">
    <b>spl_autoload_register</b> automatically loads classes.<br>
    Once write autoloader function that parses file path from class namespace and<br>
    You will never have to include every php files manually with functions like "require".
</div>


```php
// function contains logic of parsing file path from namespace
function myAutoLoader($className) {
    require str_replace("\\", DIRECTORY_SEPARATOR, $className) . '.php';
}

spl_autoload_register('myAutoLoader');

$db = new \models\db\DbConnection();
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/16/php-curl">
                php curl
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/16/php-recursive-mkdir">
                php recursive mkdir
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/16/php-recursive-mkdir">
                php recursive mkdir
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/15/php-array_merge">
                php array_merge
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/15/php-change-file-permissions">
                php change file permissions
            </a>
        </li>
    </ul>
</div>