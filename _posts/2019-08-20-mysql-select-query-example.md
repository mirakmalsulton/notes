---
title: PHP - mysql select query example
---

<h1 class="header">PHP - mysql select query example</h1>

```php
$db = mysqli_connect('host', 'dbUser', 'dbPassword', 'dbName');
$query = $db->query("SELECT * FROM `country`");
while($row = $query->fetch_assoc()) {
    echo $row['id'] . '|' . $row['name'] . '<br>' . PHP_EOL;
}

// output
// 1|France
// 2|Russia
// 3|Italy
// 4|Spain
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/09/01/php-round-up-round-down-example">
                php round up round down example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/php-header-utf8">
                php header utf8
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/php-recursive-directory-delete">
                php recursive directory delete
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/php-script-exec-time">
                php script exec time
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/09/php-error_reporting-all">
                php error_reporting all
            </a>
        </li>
    </ul>
</div>