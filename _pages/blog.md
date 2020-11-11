---
permalink: /blog
layout: page
title: Blog
---

<div>
    {% for post in site.posts %}
        <div>
            <small>{{post.date | date_to_string: "ordinal", "US" }}</small>
            <br>
            <a href=".{{ post.url }}">{{ post.title }}</a>
            <p>{{post.excerpt}}</p>
        </div>    
    {% endfor %}
</div>