---
title: Yii2 - hidden input value
---

<h1 class="header">Yii2 - hidden input value</h1>

<b>You can create a hidden field in two ways</b>

<i>Method 1: inside active form</i>
```php
<?php $form = ActiveForm::begin() ?>
<?= $form->field($model, 'book')->hiddenInput(['data-attr' => 'any_data'])->label(false) ?>
<?= Html::submitButton('Save', ['class' => 'btn btn-success']) ?>
<?php ActiveForm::end() ?>
```

<i>Method 2: with html helper</i>
```php
<?= Html::hiddenInput('name', $value) ?>
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
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
    </ul>
</div>