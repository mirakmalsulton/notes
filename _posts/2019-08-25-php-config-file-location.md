---
title: PHP - config file location
---

<h1 class="header">PHP - config file location</h1>

Configuration file can be located in several different areas

<h3>Method 1</h3>

Create info.php with code above and open the file in your browser
```php
<?php
phpinfo();
```

You will see the path to the php.ini like in the following screenshot
<div style="margin-bottom: 40px;">
    <img src="{{ site.baseurl }}/images/php-config-file-location.png"
    style="border: 1px solid #ddd"
    alt="php config file location">
</div>


<h3>Method 2</h3>

For Linux based OS
```code
php -i | grep "Loaded Configuration File"
```

For Windows
```code
php -i | findstr /c:"Loaded Configuration File"
```

Output should be something like this
```code
Loaded Configuration File => /etc/php/7.2/cli/php.ini
```