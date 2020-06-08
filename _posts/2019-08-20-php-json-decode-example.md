---
title: PHP - json decode example
---

<h1 class="header">PHP - json decode example</h1>

json to object
```php
$json = '{"a":1,"b":2,"c":[1,2]}';
$out = json_decode($json);
print_r($out);
// output
// stdClass Object
// (
//     [a] => 1
//     [b] => 2
//     [c] => Array
//         (
//             [0] => 1
//             [1] => 2
//         )
// )
```

json to array
```php
$json = '{"a":1,"b":2,"c":[1,2]}';
$out = json_decode($json, true);
print_r($out);
// output
// Array
// (
//     [a] => 1
//     [b] => 2
//     [c] => Array
//         (
//             [0] => 1
//             [1] => 2
//         )
// )
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
            <a href="https://mirakmalsulton.github.io/notes/2019/08/10/php-get-current-working-directory">
                php get current working directory
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/10/php-get-file-size">
                php get file size
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/15/php-chown">
                php chown
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/15/php-chgrp">
                php chgrp
            </a>
        </li>
    </ul>
</div>