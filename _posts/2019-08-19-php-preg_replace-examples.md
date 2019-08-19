---
title: PHP - preg_replace examples
---

<h1 class="header">PHP - preg_replace examples</h1>

```php
$string = 'May 11, 2019';
$pattern = '/(\w+) (\d+), (\d+)/i';
$replacement = '${1} 3, 2020';
echo preg_replace($pattern, $replacement, $string);
// output
// May 3, 2020
```


```php
$string = 'September 2, 2018';
$pattern = '([0-9]{4})';
$replacement = '2020';
echo preg_replace($pattern, $replacement, $string);
// output
// September 2, 2020
```


```php
$string = 'September 2, 2019';
$pattern = '/\w+ \d/';
$replacement = 'June 8';
echo preg_replace($pattern, $replacement, $string);
// output
// June 8, 2019
```