---
title: PHP - change file permissions
---

<h1 class="header">PHP - change file permissions</h1>

changes the owner of the file
```php
chown('/path/to/file', 'user_name');
```

changes the usergroup of the file
```php
chgrp('/path/to/file', 'user_name');
```

changes the permissions of the file
```php
chmod('/path/to/file', 0777);
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/06/linux-chmod-command">
                linux chmod command
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/06/linux-if-dir-not-exists-create">
                linux if dir not exists create
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/06/linux-ls-hidden-files">
                linux ls hidden files
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/linux-copy-folders-with-files">
                linux copy folders with files
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/linux-create-dir-with-permissions">
                linux create dir with permissions
            </a>
        </li>
    </ul>
</div>