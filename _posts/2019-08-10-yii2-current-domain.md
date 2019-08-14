---
title: Yii2 - get current domain
---

<h1 class="header">Yii2 - get current domain</h1>

```php
use yii\helpers\Url;
Url::base(); // /myapp
Url::base(true); // http(s)://example.com/myapp - depending on current schema
Url::base('https'); // https://example.com/myapp
Url::base('http'); // http://example.com/myapp
Url::base(''); // //example.com/myapp
```