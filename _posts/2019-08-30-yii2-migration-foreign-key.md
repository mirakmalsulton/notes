---
title: Yii2 - andFilterWhere
---

<h1 class="header">Yii2 - andFilterWhere</h1>

<div style="color:#555;margin-bottom:30px;">
    A FOREIGN KEY is a key used to link two tables together.
</div>


Syntax
```php
$this->addForeignKey(name, table, column, referringTable, referringColumn, delete, update);
// delete options: RESTRICT, CASCADE, NO ACTION, SET DEFAULT, SET NULL
// update options: RESTRICT, CASCADE, NO ACTION, SET DEFAULT, SET NULL
```


Add foreign key
```php
public function safeUp()
{
    $this->createTable('book', [
        'id' => $this->primaryKey(),
        'name' => $this->string(255)->notNull(),
        'categoryId' => $this->integer(11)->notNull(),
        'price' => $this->integer(11)->notNull(),
        'status' => $this->integer(1)->notNull(),
    ]);

    $this->addForeignKey('fk-categoryId', 'book', 'categoryId', 'category', 'id', 'RESTRICT', 'RESTRICT');
}
```

Drop foreign key
```php
$this->dropForeignKey('fk-categoryId', 'book');
```