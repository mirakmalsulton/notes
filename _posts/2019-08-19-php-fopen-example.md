---
title: PHP - fopen example
---

<h1 class="header">PHP - fopen example</h1>

Syntax
```code
fopen(pathToFile, mode);
```

Example
```php
$handle = fopen('/path/to/file.txt', 'r');
while (!feof($file)) {
    $line = fgets($file);
    echo $line;
}
fclose($file);
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/24/php-send-email-with-attachment-example">
                php send email with attachment example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/24/php-move_uploaded_file-example">
                php move_uploaded_file example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/24/php-usort-example">
                php usort example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/25/php-scandir-example">
                php scandir example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/25/php-xpath-query-examples">
                php xpath query examples
            </a>
        </li>
    </ul>
</div>