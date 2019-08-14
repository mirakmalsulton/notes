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