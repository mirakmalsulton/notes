---
title: PHP - strtotime example
---

<h1 class="header">PHP - strtotime example</h1>

<div style="color:#555;margin-bottom:30px;">
    <b>strtotime</b> - Converts textual datetime into Unix timestamp.
</div>


Separator is a dot (.), European  date format (only 4 digit years)
```php
echo date('jS F, Y', strtotime('11.12.2013')) . '\n';
// outputs 11th December, 2013
```

Separator is a slash (/), American date format
```php
echo date('jS F, Y', strtotime('11/12/13')) . '\n';
// outputs 12th November, 2013
```

Separator is a dash (-), European  date format
```php
echo date('jS F, Y', strtotime('13-12-11')) . '\n';
// outputs 11th December, 2013
```

```php
echo strtotime('now'), '\n';
echo strtotime('10 June 2019'), '\n';
echo strtotime('+1 day'), '\n';
echo strtotime('+1 week'), '\n';
echo strtotime('+1 week 5 days 3 hours 3 seconds'), '\n';
echo strtotime('next Friday'), '\n';
echo strtotime('last Sunday'), '\n';
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
            <a href="https://mirakmalsulton.github.io/notes/2019/08/16/php-strpos-example">
                php strpos example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/16/php-ping-ip-or-domain">
                php ping ip or domain
            </a>
        </li>
    </ul>
</div>