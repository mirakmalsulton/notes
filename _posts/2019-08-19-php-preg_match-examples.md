---
title: PHP - preg_match examples
---

<h1 class="header">PHP - preg_match examples</h1>

```php
preg_match('/(hello) (world)/', 'hello world!', $matches);
print_r($matches);
// output
// Array
// (
//     [0] => hello world
//     [1] => hello
//     [2] => world
// )
```

```php
preg_match('/world/', 'hello world!', $matches);
print_r($matches);
// output
// Array
// (
//     [0] => world
// )
```

```php
preg_match('/abc/', 'hello world!', $matches);
print_r($matches);
// output
// Array
// (
// )
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/25/php-config-file-location">
                php config file location
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-ob_start-example">
                php ob_start example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-hashing-example-sha256-sha1-md5">
                php hashing example sha256 sha1 md5
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-str_replace-example">
                php str_replace example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-recursive-function-example">
                php recursive function example
            </a>
        </li>
    </ul>
</div>