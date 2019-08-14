---
title: PHP - script execution time
---

<h1 class="header">PHP - script execution time</h1>

```php
$execStart = microtime(true);
//Your code here
echo 'Execution time: ' . (microtime(true) - $execStart);
```