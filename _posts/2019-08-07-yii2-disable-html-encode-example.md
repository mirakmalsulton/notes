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


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/yii2-form-validation-rules-length">
            yii2 form validation rules length
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/yii2-hidden-input-value">
                yii2 hidden input value
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/yii2-render-image">
                yii2 render image
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/yii2-submit-button-confirm">
                yii2 submit button confirm
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/javascript-get-data-attribute">
                javascript get data attribute
            </a>
        </li>
    </ul>
</div>