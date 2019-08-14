---
title: Yii2 - render image
---

<h1 class="header">Yii2 - render image</h1>

```php
public function actionIndex()
{
    $response = Yii::$app->getResponse();
    $response->headers->set('Content-Type', 'image/jpeg');
    $response->format = Response::FORMAT_RAW;
    $response->stream = fopen(Yii::getAlias('@app/web/picture.jpg'), 'r');
    $response->send();
}
```