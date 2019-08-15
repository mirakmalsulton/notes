---
title: PHP - change file permissions
---

<h1 class="header">PHP - chmod</h1>

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