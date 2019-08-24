---
title: PHP - send email with attachment example
---

<h1 class="header">PHP - send email with attachment example</h1>

<ul>
    <li>Install <b>composer</b> if doesn't already exists</li>
    <li>Install phpmailer library with command - <b>composer require phpmailer/phpmailer</b></li>
    <li>Copy the code from above and paste it into your index.php file</li>
    <li>Execute created file with command - <b>php index.php</b></li>
</ul>

```php
require 'vendor/autoload.php';

use PHPMailer\PHPMailer\PHPMailer;

$email = new PHPMailer(true);

try {
    $email->Subject = 'Cartoon';
    $email->Body = 'Hello Tom!.';
    $email->AddAttachment('path/to/file.txt', 'fileName.txt');
    $email->setFrom('yourmail@gmail.com', 'Jerry');
    $email->addAddress('clientmail@mail.ru', 'Tom');
    $email->send();
} catch (PHPMailer\PHPMailer\Exception $e) {
    echo $e->errorMessage();
} catch (\Exception $e) {
    echo $e->getMessage();
}
```