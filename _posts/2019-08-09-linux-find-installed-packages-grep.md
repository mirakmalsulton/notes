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


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/15/linux-chown">
                linux chown
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/10/linux-nano-save">
                linux nano save
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/linux-move-directory">
                linux move directory
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/linux-check-if-dir-exists">
                linux check if dir exists
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/linux-zip-folder">
                linux zip folder
            </a>
        </li>
    </ul>
</div>