---
title: PHP - send mail using gmail smtp
---

<h1 class="header">PHP - send mail using gmail smtp</h1>

<ul>
    <li>
        Go to the https://myaccount.google.com/lesssecureapps and enable "Allow less secure apps"
    </li>
    <li>
        install <b>composer</b> if doesn't already exists
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
    $mail->isSMTP();
    $mail->SMTPAuth = true;
    $mail->SMTPSecure = 'tls';
    $mail->Port = 587;
    $mail->Host = 'smtp.gmail.com';
    $mail->Username = 'yourgmail@gmail.com';
    $mail->Password = 'yourgmailpassword';

    $mail->setFrom('yourgmail@gmail.com', 'Superman');
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