---
title: PHP - spl_autoload_register example
---

<h1 class="header">PHP - spl_autoload_register example</h1>

<div style="color:#555;margin-bottom:30px;">
    <b>spl_autoload_register</b> automatically loads classes.<br>
    Once write autoloader function that parses file path from class namespace and<br>
    You will never have to include every php files manually with functions like "require".
</div>


```php
// function contains logic of parsing file path from namespace
function myAutoLoader($className) {
    require str_replace("\\", DIRECTORY_SEPARATOR, $className) . '.php';
}

spl_autoload_register('myAutoLoader');

$db = new \models\db\DbConnection();
```