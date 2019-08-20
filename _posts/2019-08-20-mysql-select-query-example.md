---
title: PHP - mysql select query example
---

<h1 class="header">PHP - mysql select query example</h1>

json to object
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