---
title: PHP - str_replace example
---

<h1 class="header">PHP - str_replace example</h1>


Syntax
```php
str_replace($find, $replace, $string, $count)
```

Example 1
```php
$string = 'Hello world!';
$find = 'world!';
$replace = 'foo bar!';
$result = str_replace($find, $replace, $string);
echo $result;
// output
// Hello foo bar
```


Example 2
```php
$string = 'Hello world!';
$find = 'o';
$replace = '';
$result = str_replace($find, $replace, $string, $count);
print_r($count);
// output
// 2
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/09/php-pdo-prepare-select">
                php pdo prepare select
            </a>
        </li>
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
    </ul>
</div>