---
permalink: /
title: Hi there
layout: page
---

👋🏾 I am a Software Engineer interested in building teams that are high performing, autonomous and mission-driven.

Keeping the codebase clean and simple with every line of code modified (or even better, removed!) is what passionates me.

Some would say <a target="_blank" href="https://en.wikipedia.org/wiki/Brownfield_(software_development)">brownfields</a> are my guilty pleasure.


<h3>Latest blog entries</h3>
<div>
{% for post in site.posts %}
    {% if forloop.index <= 3 %}
        <div>
            <small>{{post.date | date_to_string: "ordinal", "US" }}</small>
            <br>
            <a href=".{{ post.url }}">{{ post.title }}</a>
            <p>{{post.excerpt}}</p>
        </div> 
    {% endif %}
{% endfor %}
</div>

