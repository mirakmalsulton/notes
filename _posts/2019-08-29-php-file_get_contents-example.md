---
title: PHP - file_get_contents example
---

<h1 class="header">PHP - file_get_contents example</h1>


Example 1
```php
$content = file_get_contents('http://www.google.com/');
echo $content;
// output
// content of url
```


Example 2
```php
$content = file_get_contents('/path/to/file.txt');
echo $content;
// output
// content of file
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
            <a href="https://mirakmalsulton.github.io/notes/2019/08/15/php-chgrp">
                php chgrp
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/15/php-chown">
                php chown
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/10/php-get-file-size">
                php get file size
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/10/php-get-current-working-directory">
                php get current working directory
            </a>
        </li>
    </ul>
</div>