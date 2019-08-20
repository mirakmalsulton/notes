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