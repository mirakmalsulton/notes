---
title: Javascript - jQuery Ajax Post Method
---

<h1 class="header">Javascript - jQuery Ajax Post Method</h1>

```javascript
$.ajax({
    type: 'POST',
    url: "path/to/url",
    data: {'data': data},
    success: function (msg) {
        alert(msg);
    }
});
```