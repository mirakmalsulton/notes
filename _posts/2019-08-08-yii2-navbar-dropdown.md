---
title: Yii2 - navbar dropdown menu
---

<h1 class="header">Yii2 - navbar dropdown menu</h1>

```php
echo Nav::widget([
    'items' => [
        [
            'label' => 'Profile', 'items' =>
            [
                ['label' => 'Friends', 'url' => ['/user/friends']],
                ['label' => 'Settings', 'url' => ['/user/settings']]
            ]
        ],
    ],
]);
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/10/yii2-current-domain">
                yii2 current domain
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/10/yii2-array-helper-map">
                yii2 array helper map
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/yii2-navbar-dropdown">
                yii2 navbar dropdown
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/yii2-activerecord-tablename">
                yii2 activerecord tablename
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/yii2-hidden-input-value">
                yii2 hidden input value
            </a>
        </li>
    </ul>
</div>