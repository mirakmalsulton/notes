---
title: PHP - move_uploaded_file example
---

<h1 class="header">PHP - move_uploaded_file example</h1>


File will be stored in temporary location. Use <b>tmp_name</b> to get uploaded file temporary path.
```php
$uploaded = 'upload/directory/' . basename($_FILES['imgUpload']['name']);
if (move_uploaded_file($_FILES['imgUpload']['tmp_name'], $uploaded)) {
    echo "Success";
} else {
    echo "Fail";
}
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