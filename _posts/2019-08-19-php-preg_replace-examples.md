---
title: PHP - preg_replace examples
---

<h1 class="header">PHP - preg_replace examples</h1>

```php
$string = 'May 11, 2019';
$pattern = '/(\w+) (\d+), (\d+)/i';
$replacement = '${1} 3, 2020';
echo preg_replace($pattern, $replacement, $string);
// output
// May 3, 2020
```


```php
$string = 'September 2, 2018';
$pattern = '([0-9]{4})';
$replacement = '2020';
echo preg_replace($pattern, $replacement, $string);
// output
// September 2, 2020
```


```php
$string = 'September 2, 2019';
$pattern = '/\w+ \d/';
$replacement = 'June 8';
echo preg_replace($pattern, $replacement, $string);
// output
// June 8, 2019
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-file_put_contents-example">
                php file_put_contents example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/29/php-file_get_contents-example">
                php file_get_contents example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/29/php-strtotime-examples">
                php strtotime examples
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/29/php-spl_autoload_register-example">
                php spl_autoload_register example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/09/01/php-round">
                php round
            </a>
        </li>
    </ul>
</div>