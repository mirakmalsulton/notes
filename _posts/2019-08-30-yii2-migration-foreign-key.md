---
title: Yii2 - migration foreign key
---

<h1 class="header">Yii2 - migration foreign key</h1>

<div style="color:#555;margin-bottom:30px;">
    A <b>FOREIGN KEY</b> is a key used to link two tables together.
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


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/yii2-form-validation-rules-length">
                yii2 form validation rules length
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/yii2-disable-html-encode-example">
                yii2 disable html encode example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/30/yii2-activeform">
                yii2 activeform
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/30/yii2-migration-foreign-key">
                yii2 migration foreign key
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/30/yii2-andfilterwhere">
                yii2 andfilterwhere
            </a>
        </li>
    </ul>
</div>