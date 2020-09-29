---
title: Yii2 - andFilterWhere
---

<h1 class="header">Yii2 - andFilterWhere</h1>

<i class="text-info">
    <b>filterWhere()</b> - ignores search by empty values.<br>
    When the search is executed by two fields, for example book and author,
    if the book value is empty then filterWhere() ignores the search by book
    and the search will be executed only by author
</i>

filterWhere()
```php
$query->filterWhere([
    'author' => $author,
    'book' => null,
]);
// generated sql query
// SELECT * FROM `library` WHERE (`author` = $author)
```

<i>andFilterWhere</i> - Appends WHERE condition to the existing one.
```php
$query->where(['author' => $author]);
$query->andFilterWhere(['book' => $book]);
// generated sql query
// SELECT * FROM `library` WHERE (`author` = $author) AND (`book` = $book)
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