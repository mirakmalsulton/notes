---
title: PHP - ping ip address or domain name
---

<h1 class="header">PHP - ping ip address or domain name</h1>

```php
$host = '185.85.0.29'; // ip address or domain name
$curl = curl_init($host);
curl_setopt($curl, CURLOPT_TIMEOUT, 5);
curl_setopt($curl, CURLOPT_CONNECTTIMEOUT, 5);
curl_setopt($curl, CURLOPT_RETURNTRANSFER, true);
$data = curl_exec($curl);
$httpCode = curl_getinfo($curl, CURLINFO_HTTP_CODE);
curl_close($curl);
if ($httpCode >= 200 && $httpCode < 300) {
    echo 'success';
} else {
    echo "error";
}
```

OR

```php
$host = "185.85.0.29"; // ip address or domain name
exec('ping ' . $host, $output, $result);
print_r($output);
if ($result == 0) {
    echo "success";
} else {
    echo "error";
}
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/27/php-ob_start-example">
                php ob_start example
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/25/php-config-file-location">
                php config file location
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/25/php-xpath-query-examples">
                php xpath query examples
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/25/php-scandir-example">
                php scandir example
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/24/php-usort-example">
                php usort example
            </a>
        </li>
    </ul>
</div>