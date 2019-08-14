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