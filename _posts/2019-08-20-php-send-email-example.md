---
title: PHP - send email example
---

<h1 class="header">PHP - send email example</h1>

<ul>
    <li>
        Install <b>composer</b> if doesn't already exists
    </li>
    <li>
        Install phpmailer library with command - <b>composer require phpmailer/phpmailer</b>
    </li>
    <li>
        Copy the code from above and paste it into your index.php file
    </li>
    <li>
        Execute created file with command - <b>php index.php</b>
    </li>
</ul>

```php
require 'vendor/autoload.php';

use PHPMailer\PHPMailer\PHPMailer;

$mail = new PHPMailer(true);

try {
    $mail->setFrom('yourmail@gmail.com', 'Superman');
    $mail->addAddress('clientmail@mail.ru', 'Batman');
    $mail->Subject = 'Battle';
    $mail->Body = 'Your text here.';
    $mail->send();
} catch (PHPMailer\PHPMailer\Exception $e) {
    echo $e->errorMessage();
} catch (\Exception $e) {
    echo $e->getMessage();
}
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/15/php-chmod">
                php chmod
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/15/php-change-file-permissions">
                php change file permissions
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/15/php-array_merge">
                php array_merge
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/16/php-recursive-mkdir">
                php recursive mkdir
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/16/php-recursive-mkdir">
                php recursive mkdir
            </a>
        </li>
    </ul>
</div>