---
title: PHP - usort example
---

<h1 class="header">PHP - usort example</h1>


```php
function myFunction($a, $b)
{
    if ($a > $b) return 1;
    if ($a == $b) return 0;
    return -1;
}

$array = [2, 4, 1, 3];
usort($array, 'myFunction');
print_r($array);
// output
// Array
// (
//     [0] => 1
//     [1] => 2
//     [2] => 3
//     [3] => 4
// )
```

Visual representation on how it works
<div>
    <img src="{{ site.baseurl }}/images/php_usort.gif" style="border: 1px solid #ddd" alt="How does usort work">
</div>


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/php-header-utf8">
                php header utf8
            </a>
        </li>
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