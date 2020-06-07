---
title: PHP - exec example
---

<h1 class="header">PHP - exec example</h1>

```php
exec('ls', $out);
var_dump($out);
// output
// Array
// (
//     [0] => file_1.txt
//     [1] => file_2.txt
//     [2] => file_3.txt
// )
```


```php
exec('whoami', $out);
print_r($out);
// output
// Array
// (
//     [0] => root
// )
```


```php
exec('pwd', $out);
print_r($out);
// output
// Array
// (
//     [0] => /current/working/directory
// )
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
            <a href="https://mirakmalsulton.github.io/notes/2019/08/19/php-preg_replace-examples">
                php preg_replace examples
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/20/php-send-email-example">
                php send email example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/20/php-send-mail-using-gmail-smtp">
                php send mail using gmail smtp
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/20/php-urlencode-urldecode-example">
                php urlencode urldecode example
            </a>
        </li>
    </ul>
</div>