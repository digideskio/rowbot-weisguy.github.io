---
layout: default
title: Rowan Weismiller | Designer & Developer
---

<div class="opening">
    <h1 class="opening__title">{{ site.author.name }}</h1>
    <p class="opening__subtitle">A designer, front-end developer, and <a class="link" href="//thenachoclub.com/">nacho critic</a> making internets in Vancouver, Canada.</p>
</div>

<h2>Recent Posts</h2>
<ul class="posts two-up">
    {% for post in site.posts %}
        <li class="two-up__column">
            <a class="card" href="{{ post.url }}">
                <div class="card__emoji">
                    {{ post.emoji }}
                </div>
                <div class="card__text">
                    <h3 class="card__title">{{ post.title }}</h3>
                    <span class="card__subtitle">{{ post.date | date_to_string }}</span>
                </div>
            </a>
        </li>
    {% endfor %}
</ul>