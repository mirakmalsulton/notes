---
title: PHP - json decode example
---

<h1 class="header">PHP - json decode example</h1>

json to object
```php
$json = '{"a":1,"b":2,"c":[1,2]}';
print_r(json_decode($json));
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
print_r(json_decode($json, true));
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