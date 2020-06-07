---
title: Sql - foreign key example
---

<h1 class="header">Sql - foreign key example</h1>

```sql
CREATE TABLE product(
    id INT PRIMARY KEY,
    customer_id INT NOT NULL,
    CONSTRAINT fk-product-customer_id
    FOREIGN KEY (customer_id)
    REFERENCES customer (id)
    ON UPDATE CASCADE
    ON DELETE CASCADE
    );
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/mysql-show-users">
                mysql show users
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/09/mysql-drop-database">
                mysql drop database
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/10/sql-foreign-key-example">
                sql foreign key example
            </a>
        </li>
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
    </ul>
</div>