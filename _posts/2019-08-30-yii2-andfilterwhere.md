---
title: Yii2 - andFilterWhere
---

<h1 class="header">Yii2 - andFilterWhere</h1>

<div style="color:#555;margin-bottom:30px;">
    <b>andFilterWhere</b> - Appends WHERE condition to the existing one.
</div>


```php
$model = Book::find()->where(['status' => 1])->andWhere(['<', 'price', 100])->one();
// generated sql query
// SELECT * FROM `book` WHERE (`status` = 1) AND (`price` < 100)
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/25/php-xpath-query-examples">
                php xpath query examples
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/25/php-scandir-example">
                php scandir example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/24/php-usort-example">
                php usort example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/24/php-move_uploaded_file-example">
                php move_uploaded_file example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/24/php-send-email-with-attachment-example">
                php send email with attachment example
            </a>
        </li>
    </ul>
</div>