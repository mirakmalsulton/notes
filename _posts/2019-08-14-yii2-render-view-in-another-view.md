---
title: Yii2 - render view in another view
---

<h1 class="header">Yii2 - render view in another view</h1>

view_1.php
```php
<?php echo $this->render('view_2', ['hello' => 'hello world']) ?>
```

view_2.php
```php
<?php
echo $hello;
// output
// hello world
?>
```