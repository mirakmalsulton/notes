---
title: Yii2 - update query
---

<h1 class="header">Yii2 - update query</h1>

```php
$connection->createCommand()
    ->update('tbl_user', ['status' => 1], 'age > 30')
    ->execute();
```