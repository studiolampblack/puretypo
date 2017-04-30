---
layout: page
title: Archive
navigation: True
logo: 'assets/images/ghost.png'
current: archive
cover: 'assets/images/cover1.jpg'
permalink: /archive/
---

A blog is usually made with a dream to be a big reference resource. Given that I have a rule that the posts should not exceed 500 or 600 words, the number of posts would be high on any given subject. So I'm collating all the topics based on the tags. This would be manually updated until I learn how to programmatically do that here&mdash;new to Jekyll. :smile:

- [PowerShell posts](http://typo.midnightlamp.black/tag/powershell)
- [Gotcha posts](http://typo.midnightlamp.black/tag/gotcha)

Also listed here are the posts, in reverse chronological order:

<section class="archive-post-list">

   {% for post in site.posts %}
       {% assign currentDate = post.date | date: "%Y" %}
       {% if currentDate != myDate %}
           {% unless forloop.first %}</ul>{% endunless %}
           <p>{{ currentDate }}</p>
           <ul>
           {% assign myDate = currentDate %}
       {% endif %}
       <li><a href="{{ post.url }}"><span>{{ post.date | date: "%B %-d, %Y" }}</span> - {{ post.title }}</a></li>
       {% if forloop.last %}</ul>{% endif %}
   {% endfor %}

</section>
