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