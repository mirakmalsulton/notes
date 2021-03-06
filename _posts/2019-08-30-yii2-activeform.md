---
title: Yii2 - ActiveForm example
---

<h1 class="header">Yii2 - ActiveForm example</h1>

<i>ActiveForm with model</i>
```php
<?php $form = ActiveForm::begin() ?>
<?= $form->field($model, 'username')->textInput() ?>
<?= $form->field($model, 'password')->passwordInput() ?>
<?= Html::submitButton('Login', ['class' => 'btn btn-primary', 'name' => 'login-button']) ?>
<?php ActiveForm::end() ?>
```


<i>ActiveForm with model and custom url</i>
```php
<?php $form = ActiveForm::begin(['action' => ['site/login']]) ?>
<?= $form->field($model, 'username')->textInput() ?>
<?= $form->field($model, 'password')->passwordInput() ?>
<?= Html::submitButton('Login', ['class' => 'btn btn-primary', 'name' => 'login-button']) ?>
<?php ActiveForm::end() ?>
```

<i>ActiveForm without model</i>
```php
<?= Html::beginForm() ?>
<label>Username</label>
<?= Html::input('text', 'LoginForm[username]', null, ['class' => 'form-group form-control']) ?>
<label>Password</label>
<?= Html::input('text', 'LoginForm[password]', null, ['class' => 'form-group form-control']) ?>
<?= Html::submitButton('Login', ['class' => 'btn btn-primary form-group']) ?>
<?= Html::endForm() ?>
```

<i>ActiveForm without model and custom url</i>
```php
<?= Html::beginForm(['site/login'], 'post') ?>
<label>Username</label>
<?= Html::input('text', 'LoginForm[username]', null, ['class' => 'form-group form-control']) ?>
<label>Password</label>
<?= Html::input('text', 'LoginForm[password]', null, ['class' => 'form-group form-control']) ?>
<?= Html::submitButton('Login', ['class' => 'btn btn-primary form-group']) ?>
<?= Html::endForm() ?>
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/20/php-json-decode-example">
                php json decode example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/20/php-urlencode-urldecode-example">
                php urlencode urldecode example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/20/php-send-mail-using-gmail-smtp">
                php send mail using gmail smtp
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/20/php-send-email-example">
                php send email example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/19/php-preg_replace-examples">
                php preg_replace examples
            </a>
        </li>
    </ul>
</div>