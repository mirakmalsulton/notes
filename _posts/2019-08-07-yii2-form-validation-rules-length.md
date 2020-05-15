---
title: Yii2 - form validation rules - length
---

<h1 class="header">Yii2 - form validation rules - length</h1>

```php
public function rules()
{
    return [
        ['property', 'string', 'max' => 10, 'tooLong' => 'Error message']
    ];
}
```


<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/yii2-activerecord-tablename">
                yii2 activerecord tablename
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/yii2-navbar-dropdown">
                yii2 navbar dropdown
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/yii2-update-query">
                yii2 update query
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/09/yii2-remove-no-results-found">
                yii2 remove no results found
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/09/yii2-render-without-layout">
                yii2 render without layout
            </a>
        </li>
    </ul>
</div>