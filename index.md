---
title: My notes
---

<div class="main">
    <div class="row">
        <div class="col-lg-12">
            <div class="card mb-4">
                <div class="list-group list-group-flush">
                    {% for post in site.posts %}
                    <a class="list-group-item list-group-item-action" href="{{ page.url | remove: '.html' | prepend: site.baseurl }}">
                        {{ post.title }}
                    </a>
                    {% endfor %}
                </div>
            </div>
        </div>
    </div>
</div>