---
title: Yii2 - remove "No results" found on GridView
---

<h1 class="header">Yii2 - remove "No results" found on GridView</h1>

```php
GridView::widget([
    'dataProvider' => $dataProvider,
    'summary' => false,
    'columns' => [
        'id',
        'book',
    ],
]);
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