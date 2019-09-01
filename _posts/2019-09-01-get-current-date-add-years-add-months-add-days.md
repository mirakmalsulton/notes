---
title: PHP - get current date, add years/months/days
---

<h1 class="header">PHP - get current date, add years/months/days</h1>


```php
$dateTime = new \DateTime('now', new \DateTimeZone('Europe/Dublin'));

//get current datetime
echo $dateTime->format('Y-m-d H:i:s');

//get current year
echo $dateTime->format('Y');

//get current month
echo $dateTime->format('m');

//get current day
echo $dateTime->format('d');
```


<b>add years to date</b>
```php
$dateTime = new \DateTime('2019-09-01 11:12:13', new \DateTimeZone('Europe/Dublin'));
$dateTime->modify('+3 year');
echo $dateTime->format('Y-m-d H:i:s');
```


<b>add months to date</b>
```php
$dateTime = new \DateTime('2019-09-01 11:12:13', new \DateTimeZone('Europe/Dublin'));
$dateTime->modify('+3 month');
echo $dateTime->format('Y-m-d H:i:s');
```


<b>add days to date</b>
```php
$dateTime = new \DateTime('2019-09-01 11:12:13', new \DateTimeZone('Europe/Dublin'));
$dateTime->modify('+3 day');
echo $dateTime->format('Y-m-d H:i:s');
```