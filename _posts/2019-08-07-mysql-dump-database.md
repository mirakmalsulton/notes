---
title: Sql - mysql dump database
---

<h1 class="header">Sql - mysql dump database</h1>

Back up a Database
```code
mysqldump -u [username] -p db_name > backup.sql
```

Restore a Backup
```code
mysql -u [username] -p < backup.sql
```