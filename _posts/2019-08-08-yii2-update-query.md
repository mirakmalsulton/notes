---
title: Yii2 - update query
---

<h1 class="header">Yii2 - update query</h1>

```php
$connection->createCommand()
    ->update('tbl_user', ['status' => 1], 'age > 30')
    ->execute();
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/yii2-disable-html-encode-example">
                yii2 disable html encode example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/yii2-activerecord-tablename">
                yii2 activerecord tablename
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/09/yii2-remove-no-results-found">
                yii2 remove no results found
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/09/yii2-render-without-layout">
                yii2 render without layout
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/10/yii2-array-helper-map">
                yii2 array helper map
            </a>
        </li>
    </ul>
</div>