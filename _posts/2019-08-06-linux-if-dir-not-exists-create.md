---
title: Linux - create if directory does not exists
---

<h1 class="header">Linux - create if directory does not exists</h1>

```code
[ -d /var/www/my_dir ] && echo "Directory exists" || mkdir /var/www/my_dir
```