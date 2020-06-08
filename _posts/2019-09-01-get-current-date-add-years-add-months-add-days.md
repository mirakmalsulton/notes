---
title: PHP - get current date, add years/months/days
---

<h1 class="header">PHP - get current date, add years/months/days</h1>


<h5>get current datetime</h5>
```php
$dateTime = new \DateTime('now', new \DateTimeZone('Europe/Dublin'));
echo $dateTime->format('Y-m-d H:i:s');
```


<h5>get current year</h5>
```php
$dateTime = new \DateTime('now', new \DateTimeZone('Europe/Dublin'));
echo $dateTime->format('Y');
```


<h5>get current month</h5>
```php
$dateTime = new \DateTime('now', new \DateTimeZone('Europe/Dublin'));
echo $dateTime->format('m');
```


<h5>get current day</h5>
```php
$dateTime = new \DateTime('now', new \DateTimeZone('Europe/Dublin'));
echo $dateTime->format('d');
```


<h5>add years to date</h5>
```php
$dateTime = new \DateTime('2019-09-01 11:12:13', new \DateTimeZone('Europe/Dublin'));
$dateTime->modify('+3 year');
echo $dateTime->format('Y-m-d H:i:s');
```


<h5>add months to date</h5>
```php
$dateTime = new \DateTime('2019-09-01 11:12:13', new \DateTimeZone('Europe/Dublin'));
$dateTime->modify('+3 month');
echo $dateTime->format('Y-m-d H:i:s');
```


<h5>add days to date</h5>
```php
$dateTime = new \DateTime('2019-09-01 11:12:13', new \DateTimeZone('Europe/Dublin'));
$dateTime->modify('+3 day');
echo $dateTime->format('Y-m-d H:i:s');
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/10/php-get-current-working-directory">
                php get current working directory
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/09/php-pdo-prepare-select">
                php pdo prepare select
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/09/php-error_reporting-all">
                php error_reporting all
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/php-script-exec-time">
                php script exec time
            </a>
        </li>
		<li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/php-recursive-directory-delete">
                php recursive directory delete
            </a>
        </li>
    </ul>
</div>