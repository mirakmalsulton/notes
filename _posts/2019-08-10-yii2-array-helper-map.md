---
title: Yii2 - ArrayHelper::map
---

<h1 class="header">Yii2 - ArrayHelper::map</h1>

```php
$array = [
    ['id' => '1', 'data' => 'value 1', 'class' => 'a'],
    ['id' => '2', 'data' => 'value 2', 'class' => 'a'],
    ['id' => '3', 'data' => 'value 3', 'class' => 'b'],
];
```

```php
$result = ArrayHelper::map($array, 'id', 'data');
// result:
// [
//     '1' => 'value 1',
//     '2' => 'value 2',
//     '3' => 'value 3',
// ]
```

```php
$result = ArrayHelper::map($array, 'id', 'data', 'class');
// result:
// [
//     'a' => [
//         '1' => 'value 1',
//         '2' => 'value 2',
//     ],
//     'b' => [
//         '3' => 'value 3',
//     ],
// ]
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/10/yii2-last-insert-id">
                yii2 last insert id
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/14/yii2-render-view-in-another-view">
                yii2 render view in another view
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/30/yii2-andfilterwhere">
                yii2 andfilterwhere
            </a>
        </li>
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
    </ul>
</div>