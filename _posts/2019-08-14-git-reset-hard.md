---
title: Git - reset hard
---

<h1 class="header">Git - reset hard</h1>

syntax
```code
git reset --hard [SOME-COMMIT-HASH]
```

example 1 (revert to the specified commit)
```code
git reset --hard 029f66f
```

example 2 (revert to a previous commit)
```code
git reset --hard HEAD
```