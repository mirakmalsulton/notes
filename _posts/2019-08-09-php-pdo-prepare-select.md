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