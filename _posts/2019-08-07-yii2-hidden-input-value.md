---
title: Yii2 - hidden input value
---

<h1 class="header">Yii2 - hidden input value</h1>

ActiveForm
```php
$form->field($model, 'book')->hiddenInput(['data-attr' => 'any_data'])->label(false);
```

Helper html
```php
$form->field($model, 'book')->hiddenInput(['data-attr' => 'any_data'])->label(false);
```