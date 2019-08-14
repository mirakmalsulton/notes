---
title: Yii2 - render view without layout
---

<h1 class="header">Yii2 - render view without layout</h1>

```php
public function actionIndex()
{
    $this->renderPartial('view');
}
```