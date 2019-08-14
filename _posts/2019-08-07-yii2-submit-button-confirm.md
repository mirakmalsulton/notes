---
title: Yii2 - submit button confirm
---

<h1 class="header">Yii2 - submit button confirm</h1>

```php
Html::submitButton('Remove', [
    'class' => 'btn btn-danger',
    'data-confirm' => 'Are you sure?'
]);
```