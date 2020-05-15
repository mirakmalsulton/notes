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


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/30/yii2-migration-foreign-key">
            yii2 migration foreign key
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/30/yii2-activeform">
            yii2 activeform
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/yii2-disable-html-encode-example">
                yii2 disable html encode example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/yii2-form-validation-rules-length">
                yii2 form validation rules length
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/yii2-hidden-input-value">
                yii2 hidden input value
            </a>
        </li>
    </ul>
</div>