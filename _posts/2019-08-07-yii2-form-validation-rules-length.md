---
title: Yii2 - form validation rules - length
---

<h1 class="header">Yii2 - form validation rules - length</h1>

```php
public function rules()
{
    return [
        ['property', 'string', 'max' => 10, 'tooLong' => 'Error message']
    ];
}
```