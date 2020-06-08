---
title: PHP - urlencode / urldecode example
---

<h1 class="header">PHP - urlencode / urldecode example</h1>

urlencode
```php
$url = 'https://google.com/search?q=hello world';
echo urlencode($url);
// output
// https%3A%2F%2Fgoogle.com%2Fsearch%3Fq%3Dhello+world
```

urldecode
```php
$url = 'https%3A%2F%2Fgoogle.com%2Fsearch%3Fq%3Dhello+world';
echo urldecode($url);
// output
// https://google.com/search?q=hello world
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