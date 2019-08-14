---
title: Yii2 - ActiveRecord table name
---

<h1 class="header">Yii2 - ActiveRecord table name</h1>

```php
class Book extends \yii\db\ActiveRecord
{
    public static function tableName()
    {
        return 'book';
    }
}
```