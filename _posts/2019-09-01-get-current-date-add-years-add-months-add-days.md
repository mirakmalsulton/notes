---
title: PHP - get current date, add years/months/days
---

<h1 class="header">PHP - get current date, add years/months/days</h1>


get current datetime
```php
$dateTime = new \DateTime('now', new \DateTimeZone('Europe/Dublin'));
echo $dateTime->format('Y-m-d H:i:s');
```


<b>get current year</b>
```php
$dateTime = new \DateTime('now', new \DateTimeZone('Europe/Dublin'));
echo $dateTime->format('Y');
```


<b>get current month</b>
```php
$dateTime = new \DateTime('now', new \DateTimeZone('Europe/Dublin'));
echo $dateTime->format('m');
```


<b>get current day</b>
```php
$dateTime = new \DateTime('now', new \DateTimeZone('Europe/Dublin'));
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