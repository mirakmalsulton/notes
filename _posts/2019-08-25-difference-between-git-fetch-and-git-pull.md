---
title: GIT - difference between "git fetch" and "git pull"
---

<h1 class="header">GIT - difference between "git fetch" and "git pull"</h1>


git fetch downloads new data from a remote repository but it does not merge
```code
git fetch origin
```

git pull downloads new data from a remote repository and merges it
```code
git pull origin master
```

Graphical representation for beginners
<div>
    <img src="{{ site.baseurl }}/images/difference-between-git-fetch-and-git-pull.png"
    style="border: 1px solid #ddd"
    alt="difference between git fetch and git pull">
</div>