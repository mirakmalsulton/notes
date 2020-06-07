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


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/yii2-update-query">
                yii2 update query
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/09/yii2-remove-no-results-found">
                yii2 remove no results found
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/09/yii2-render-without-layout">
                yii2 render without layout
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/10/yii2-array-helper-map">
                yii2 array helper map
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/10/yii2-current-domain">
                yii2 current domain
            </a>
        </li>
    </ul>
</div>