---
title: PHP - array_merge
---

<h1 class="header">PHP - array_merge</h1>

```php
$array1 = ['a', 'b', 'c'];
$array2 = ['d', 'e', 'f'];

$array3 = array_merge($array1, $array2);

var_dump($array3);
```

output
```code
array(6) {
  [0] =>
  string(1) "a"
  [1] =>
  string(1) "b"
  [2] =>
  string(1) "c"
  [3] =>
  string(1) "d"
  [4] =>
  string(1) "e"
  [5] =>
  string(1) "f"
}
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/linux-find-a-file">
                linux find a file
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/linux-zip-folder">
                linux zip folder
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/linux-check-if-dir-exists">
                linux check if dir exists
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/linux-move-directory">
                linux move directory
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/linux-recursively-create-directory">
                linux recursively create directory
            </a>
        </li>
    </ul>
</div>