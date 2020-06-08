---
title: PHP - scandir example
---

<h1 class="header">PHP - scandir example</h1>

Ascending order
```php
$files = scandir('/path/to/dir');
print_r($files);
// output
// Array
// (
//     [0] => .
//     [1] => ..
//     [2] => bar.php
//     [3] => foo.txt
//     [4] => someFolder
// )
```


Descending order
```php
$files = scandir('/path/to/dir', 1);
print_r($files);
// Array
// (
//     [0] => someFolder
//     [1] => foo.txt
//     [2] => bar.php
//     [3] => ..
//     [4] => .
// )
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/16/php-ping-ip-or-domain">
                php ping ip or domain
            </a>
        </li>
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
    </ul>
</div>