---
title: Htaccess - Redirect all requests to index
---

<h1 class="header">Htaccess - Redirect all requests to index</h1>

```apache
Order Allow,Deny
Allow from all

AddDefaultCharset utf-8

RewriteEngine on

RewriteCond %{REQUEST_FILENAME} !-f
RewriteCond %{REQUEST_FILENAME} !-d
RewriteRule . index.php
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/15/php-chown">
                php chown
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/15/php-chgrp">
                php chgrp
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/15/php-chmod">
                php chmod
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/15/php-change-file-permissions">
                php change file permissions
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/15/php-array_merge">
                php array_merge
            </a>
        </li>
    </ul>
</div>