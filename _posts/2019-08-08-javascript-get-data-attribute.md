---
title: Javascript - get data attribute
---

<h1 class="header">Javascript - get data attribute</h1>

```html
<span id="hello" data-hello="hello world"></span>
```
```javascript
var data = document.getElementById('hello').getAttribute('data-hello');
```