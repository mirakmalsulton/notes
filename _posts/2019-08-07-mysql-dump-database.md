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


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/19/mysqli_connect-example">
                mysqli_connect example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/20/mysql-select-query-example">
                mysql select query example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/06/mysql-get-count">
                mysql get count
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/mysql-dump-database">
                mysql dump database
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/mysql-show-users">
                mysql show users
            </a>
        </li>
    </ul>
</div>