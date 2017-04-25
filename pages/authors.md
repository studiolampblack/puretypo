---
layout: page
title: Authors
navigation: True
logo: 'assets/images/ghost.png'
current: authors
cover: 'assets/images/cover1.jpg'
permalink: /authors/
---
{% for author in site.authors %}
  <div class="author-group">
    {% assign main-auth = author | first %}
    {% assign author_name = author | last %}
    <div id="#{{ main-auth | slugize }}"></div>
    <h3 class="author-head">{{ author_name.displayname }}</h3>
        {% for post in site.posts %}
            {% if post.author == main-auth %}
                <li style="list-style: none"><a target="_blank" href="{{post.url}}">{{ post.title }}</a></li>
            {% endif %}
        {% endfor %}
  </div>
{% endfor %
