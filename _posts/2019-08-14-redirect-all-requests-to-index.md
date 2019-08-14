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