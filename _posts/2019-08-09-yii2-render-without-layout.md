---
title: Yii2 - render view without layout
---

<h1 class="header">Yii2 - render view without layout</h1>

<p>
	You have to use "renderPartial" to exclude layout from view.<br>
	But "renderPartial" prevents loading asset files like css and js.<br>
	Take a look at the example below.
</p>

```php
public function actionIndex()
{
    $this->renderPartial('view', ['model' => $yourModel]);
}
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