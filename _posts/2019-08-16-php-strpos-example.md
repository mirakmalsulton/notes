---
title: PHP - strpos example
---

<h1 class="header">PHP - strpos example</h1>

Find the position of the first occurrence of a substring in a string
```php
$string = 'hello world';
$post = strpos($string, 'world'); // $pos = 6
$post = strpos($string, 'o'); // $pos = 4
```

ignoring anything before the offset
```php
$string = 'hello world';
$post = strpos($string, 'o', 5); // $pos = 7
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/09/php-error_reporting-all">
                php error_reporting all
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/php-script-exec-time">
                php script exec time
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/php-recursive-directory-delete">
                php recursive directory delete
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/php-header-utf8">
                php header utf8
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/09/01/php-round-up-round-down-example">
                php round-up round down example
            </a>
        </li>
    </ul>
</div>