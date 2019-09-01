---
title: PHP - get current date, add years/months/days
---

<h1 class="header">PHP - get current date, add years/months/days</h1>


get current datetime
```php
$dateTime = new \DateTime('now', new \DateTimeZone('Europe/Dublin'));
echo $dateTime->format('Y-m-d H:i:s');
```


get current year
```php
$dateTime = new \DateTime('now', new \DateTimeZone('Europe/Dublin'));
echo $dateTime->format('Y');
```


get current month
```php
$dateTime = new \DateTime('now', new \DateTimeZone('Europe/Dublin'));
echo $dateTime->format('m');
```


get current day
```php
$dateTime = new \DateTime('now', new \DateTimeZone('Europe/Dublin'));
echo $dateTime->format('d');
```


add years to date
```php
$dateTime = new \DateTime('2019-09-01 11:12:13', new \DateTimeZone('Europe/Dublin'));
$dateTime->modify('+3 year');
echo $dateTime->format('Y-m-d H:i:s');
```


add months to date
```php
$dateTime = new \DateTime('2019-09-01 11:12:13', new \DateTimeZone('Europe/Dublin'));
$dateTime->modify('+3 month');
echo $dateTime->format('Y-m-d H:i:s');
```


add days to date
```php
$dateTime = new \DateTime('2019-09-01 11:12:13', new \DateTimeZone('Europe/Dublin'));
$dateTime->modify('+3 day');
echo $dateTime->format('Y-m-d H:i:s');
```