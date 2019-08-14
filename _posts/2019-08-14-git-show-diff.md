---
title: Git - show diff
---

<h1 class="header">Git - show diff</h1>

```php
// compare the working directory with local repository
git diff HEAD [filename]


// compare the working directory with index
git diff [filename]


// compare the index with local repository
git diff --cached [filename]


// compare files between two different commits
git diff 7eb2..e03 812...a3f35


// compares working directory with index
// shows the changes that are not staged yet
git diff


// compares working directory with local repository
// shows the list of changes after your last commit
git diff HEAD


// compares index with local repository
// shows the diff between your last commit and changes to be committed next
git diff --cached
```