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