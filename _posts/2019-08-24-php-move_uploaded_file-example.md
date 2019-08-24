---
title: PHP - move_uploaded_file example
---

<h1 class="header">PHP - move_uploaded_file example</h1>


File will be stored in temporary location. Use <b>tmp_name</b> to get uploaded file temporary path.
```php
$uploaded = 'upload/directory/' . basename($_FILES['imgUpload']['name']);
if (move_uploaded_file($_FILES['imgUpload']['tmp_name'], $uploaded)) {
    echo "Success";
} else {
    echo "Fail";
}
```