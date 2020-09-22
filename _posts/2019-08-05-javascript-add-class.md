---
title: Javascript - add class
---

<h1 class="header">Javascript - add class</h1>

```html
<span id="hello">Hello world</span>
```
```javascript
document.getElementById("hello").classList.add("class_name");
```

gaga 23

{% capture changed_url %}
  {% assign url = page.url | remove: '2019/' %}

  {% assign url = url | remove: '08/' %}
  {% assign url = url | remove: '09/' %}

  {% assign url = url | remove: '01/' %}
  {% assign url = url | remove: '05/' %}
  {% assign url = url | remove: '06/' %}
  {% assign url = url | remove: '07/' %}
  {% assign url = url | remove: '08/' %}
  {% assign url = url | remove: '09/' %}
  {% assign url = url | remove: '10/' %}
  {% assign url = url | remove: '14/' %}
  {% assign url = url | remove: '15/' %}
  {% assign url = url | remove: '16/' %}
  {% assign url = url | remove: '19/' %}
  {% assign url = url | remove: '20/' %}
  {% assign url = url | remove: '24/' %}
  {% assign url = url | remove: '25/' %}
  {% assign url = url | remove: '27/' %}
  {% assign url = url | remove: '29/' %}
  {% assign url = url | remove: '30/' %}

  {{ url }}
{% endcapture %}

ddd = {{ changed_url }}
zaza

<div class="related_posts_block">
    <h3>Related posts:</h3>

    <ul>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/05/javascript-add-class">
                javascript add class
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/07/javascript-add-style">
                javascript add style
            </a>
        </li>
        <li>
            <a href="https://mirakmalsulton.github.io/notes/2019/08/08/javascript-get-data-attribute">
                javascript get data attribute
            </a>
        </li>
    </ul>
</div>