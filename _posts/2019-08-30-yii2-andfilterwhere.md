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