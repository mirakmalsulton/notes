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
    $email->AddAttachment('path/to/file.pdf', 'fileName.pdf');
    $email->setFrom('yourmail@gmail.com', 'Jerry');
    $email->addAddress('clientmail@mail.ru', 'Tom');
    $email->send();
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
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-ob_start-example">
                php ob_start example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-hashing-example-sha256-sha1-md5">
                php hashing example sha256 sha1 md5
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-str_replace-example">
                php str_replace example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-recursive-function-example">
                php recursive function example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-file_put_contents-example">
                php file_put_contents example
            </a>
        </li>
    </ul>
</div>