---
title: PHP - urlencode / urldecode example
---

<h1 class="header">PHP - urlencode / urldecode example</h1>

urlencode
```php
$url = 'https://google.com/search?q=hello world';
echo urlencode($url);
// output
// https%3A%2F%2Fgoogle.com%2Fsearch%3Fq%3Dhello+world
```

urldecode
```php
$url = 'https%3A%2F%2Fgoogle.com%2Fsearch%3Fq%3Dhello+world';
echo urldecode($url);
// output
// https://google.com/search?q=hello world
```