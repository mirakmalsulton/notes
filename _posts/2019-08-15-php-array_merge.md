---
title: PHP - array_merge
---

<h1 class="header">PHP - array_merge</h1>

```php
$array1 = ['a', 'b', 'c'];
$array2 = ['d', 'e', 'f'];

$array3 = array_merge($array1, $array2);

var_dump($array3);
```

output
```code
array(6) {
  [0] =>
  string(1) "a"
  [1] =>
  string(1) "b"
  [2] =>
  string(1) "c"
  [3] =>
  string(1) "d"
  [4] =>
  string(1) "e"
  [5] =>
  string(1) "f"
}
```