---
title: Linux - find installed packages
---

<h1 class="header">Linux - find installed packages</h1>

Centos
```code
sudo yum list installed | grep unzip
```

Ubuntu 14.04 and above
```code
sudo apt list --installed | grep unzip
```

Ubuntu Older Versions
```ruby
dpkg --get-selections | grep unzip
```
