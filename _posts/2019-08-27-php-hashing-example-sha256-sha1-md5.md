---
title: PHP - hashing example (sha256, sha1, md5)
---

<h1 class="header">PHP - hashing example (sha256, sha1, md5)</h1>


<b>sha256</b>
```php
$password = 'ghK$*Gl3';
echo hash('sha256', $password);
// output
// 6215da7f0e0b8fbf50e62fcf30755c5dd32b5c700ba361ce60fcb735d95db020
```

<b>sha1</b>
```php
$password = 'ghK$*Gl3';
echo hash('sha1', $password);
// output
// b61911d4ef4d0a7e6e99d2d9d92b9ec80983e0c3
```

<b>md5</b>
```php
$password = 'ghK$*Gl3';
echo hash('md5', $password);
// output
// db5f2f392736771a631bb2a8066d5d6e
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/25/php-config-file-location">
                php config file location
            </a>
        </li>
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
    </ul>
</div>