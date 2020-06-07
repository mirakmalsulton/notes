---
title: PHP - pdo prepare select
---

<h1 class="header">PHP - pdo prepare select</h1>

```php
$db->beginTransaction();
$stmt = $db->prepare("SELECT * FROM `post` WHERE `id` = :id");
$stmt->execute(['id' => $id]);
$post = $stmt->fetch(PDO::FETCH_ASSOC);
$db->commit();
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
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-ob_start-example">
                php ob_start example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-hashing-example-sha256-sha1-md5">
                php hashing example sha256 sha1 md5
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-str_replace-example">
                php str_replace example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-recursive-function-example">
                php recursive function example
            </a>
        </li>
    </ul>
</div>