---
title: PHP - xPath query example
---

<h1 class="header">PHP - xPath query example</h1>


```html
<div class="my_div">
    <h1>This is h1 tag</h1>
    <span id="my_span">This is span tag</span><br>

    <p data-hello="hello_world">
        <a href="#">This is a tag</a>
    </p>

    <p data-hello="hello_world">
        <a href="my_url.php">This is a tag</a><br>
        <a href="my_url.php">This is a tag</a>
    </p>
</div>
```


```php
$html = file_get_contents('path/to/file.html'); //paste file or url

$pattern = '//div[@class="my_div"]/h1/text()';
print_r(xParser($html, $pattern));
// output
// Array
// (
//     [0] => This is h1 tag
// )

$pattern = '//div/span';
print_r(xParser($html, $pattern));
// output
// Array
// (
//     [0] => <span id="my_span">This is span tag</span>
// )

$pattern = '//p[@data-hello="hello_world"][2]/a/@href';
print_r(xParser($html, $pattern));
// output
// Array
// (
//     [0] =>  href="my_url.php"
//     [1] =>  href="my_url.php"
// )


function xParser($html, $pattern)
{
    libxml_use_internal_errors(true);
    $dom = new \DOMDocument();
    $dom->loadHTML($html);
    libxml_clear_errors();
    $xpath = new \DOMXPath($dom);
    $nodes = $xpath->query($pattern);
    $results = [];
    foreach ($nodes as $node) {
        $results[] = $dom->saveHtml($node);
    }
    return $results;
}
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/19/php-preg_replace-examples">
                php preg_replace examples
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/19/php-preg_match-examples">
                php preg_match examples
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/19/php-fopen-example">
                php fopen example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/19/php-exec-example">
                php exec example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/16/php-strpos-example">
                php strpos example
            </a>
        </li>
    </ul>
</div>