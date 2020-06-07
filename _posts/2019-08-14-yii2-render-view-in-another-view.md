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


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/10/yii2-last-insert-id">
                yii2 last insert id
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/14/yii2-render-view-in-another-view">
                yii2 render view in another view
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/30/yii2-andfilterwhere">
                yii2 andfilterwhere
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/30/yii2-migration-foreign-key">
                yii2 migration foreign key
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/30/yii2-activeform">
                yii2 activeform
            </a>
        </li>
    </ul>
</div>