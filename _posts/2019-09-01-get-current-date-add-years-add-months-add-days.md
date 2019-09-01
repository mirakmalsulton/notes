---
title: PHP - get current date, add years/months/days
---

<h1 class="header">PHP - get current date, add years/months/days</h1>


<h4>get current datetime</h4>
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