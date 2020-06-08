---
title: PHP - send mail using gmail smtp
---

<h1 class="header">PHP - send mail using gmail smtp</h1>

<ul>
    <li>
        Go to the https://myaccount.google.com/lesssecureapps and enable "Allow less secure apps"
    </li>
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


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/19/php-preg_match-examples">
                php preg_match examples
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/19/php-fopen-example">
                php fopen example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/19/php-exec-example">
                php exec example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/16/php-ping-ip-or-domain">
                php ping ip or domain
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/16/php-curl">
                php curl
            </a>
        </li>
    </ul>
</div>