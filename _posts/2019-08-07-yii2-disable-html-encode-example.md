---
title: Yii2 - disable html encode
---

<h1 class="header">Yii2 - disable html encode</h1>

In gridview
```php
GridView::widget([
    'dataProvider' => $dataProvider,
    'columns' => [
        'id',
        [
            'attribute' => 'book',
            'label' => 'Books',
            'format' => 'raw',
            'value' => function ($data) {
                return Html::img('@web/books/book_id.jpg', [
                    'alt' => 'Harry Potter', 'class' => 'my_class'
                ]);
            }
        ],
        'user_id',
    ],
]);
```

In form field
```php
$form->field($model, 'bookList')->radioList([
    1 => Html::img('@web/books/book_1.jpg'),
    2 => Html::img('@web/books/book_2.jpg')
], ['encode' => false])->label();
```