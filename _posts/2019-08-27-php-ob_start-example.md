---
title: PHP - ob_start example
---

<h1 class="header">PHP - ob_start example</h1>

Example 1
```php
ob_start(); // captures the output and save it in an internal buffer
echo("world!"); // "world!" saved in internal buffer
$output = ob_get_contents(); // save in a variable internal buffer content
ob_end_clean(); // clean internal buffer
echo 'Hello ' . $output;
// output
// Hello world!
```


Example 2
```php
ob_start();
echo("Hello world!");
$output = ob_get_contents();
ob_end_flush(); // print internal buffer content
// output
// Hello world!
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-file_put_contents-example">
                php file_put_contents example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-recursive-function-example">
                php recursive function example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-str_replace-example">
                php str_replace example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-hashing-example-sha256-sha1-md5">
                php hashing example sha256 sha1 md5
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-ob_start-example">
                php ob_start example
            </a>
        </li>
    </ul>
</div>