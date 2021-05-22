---
layout: page
title: Blog
permalink: '/blog/'
---
<div class='blog'>
    {% assign posts = site.posts | where: 'layout','post' %}
    <ul>
    {% for post in posts %}
        <li>
        <a href='{{ post.url | absolute_url }}'>
            {{ post.title }}
        </a>
        <p>
            {{ post.author }} | 
            <time datetime='{{ page.publish_date | date_to_xmlschema }}'>
                {{ post.publish_date | date: "%A, %B %d, %Y" }}
            </time>
        </p>
        </li>
    {% endfor %}
    </ul>
</div>
