---
title: Yii2 - ActiveForm example
---

<h1 class="header">Yii2 - ActiveForm example</h1>

<b>ActiveForm with model</b>
```php
<?php $form = ActiveForm::begin() ?>
<?= $form->field($model, 'username')->textInput() ?>
<?= $form->field($model, 'password')->passwordInput() ?>
<?= Html::submitButton('Login', ['class' => 'btn btn-primary', 'name' => 'login-button']) ?>
<?php ActiveForm::end() ?>
```


<b>ActiveForm without model</b>
```php
<?= Html::beginForm() ?>
<b>Username</b>
<?= Html::input('text', 'LoginForm[username]', null, ['class' => 'form-group form-control']) ?>
<b>Password</b>
<?= Html::input('text', 'LoginForm[password]', null, ['class' => 'form-group form-control']) ?>
<?= Html::submitButton('Login', ['class' => 'btn btn-primary form-group']) ?>
<?= Html::endForm() ?>
```


<b>ActiveForm custom url</b>
```php
<?= Html::beginForm(['site/login'], 'post') ?>
<b>Username</b>
<?= Html::input('text', 'LoginForm[username]', null, ['class' => 'form-group form-control']) ?>
<b>Password</b>
<?= Html::input('text', 'LoginForm[password]', null, ['class' => 'form-group form-control']) ?>
<?= Html::submitButton('Login', ['class' => 'btn btn-primary form-group']) ?>
<?= Html::endForm() ?>


<?php $form = ActiveForm::begin(['action' => ['site/login']]) ?>
<?= $form->field($model, 'username')->textInput() ?>
<?= $form->field($model, 'password')->passwordInput() ?>
<?= Html::submitButton('Login', ['class' => 'btn btn-primary', 'name' => 'login-button']) ?>
<?php ActiveForm::end() ?>
```