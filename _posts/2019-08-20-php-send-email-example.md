---
title: PHP - send email example
---

<h1 class="header">PHP - send email example</h1>

<ul>
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