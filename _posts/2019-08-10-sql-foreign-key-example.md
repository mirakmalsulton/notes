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