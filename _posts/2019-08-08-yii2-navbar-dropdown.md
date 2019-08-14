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