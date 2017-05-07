---
layout: page
title: Archive
navigation: True
logo: 'assets/images/merakipost.svg'
current: archive
cover: 'assets/images/cover1.jpg'
---

The Meraki Post team is a bunch of unconventionally busy people. We're all the time engaged in reading, getting deeper and deeper in the world of books. Think of us as Alan at the bookstore in the episode, *That Special Tug* of *Two and a Half Men*&mdash;sans the emotional breakdown, of course.

Over the years, it has led to us reading tens of titles, the reviews for which are posted here. These tens of titles could quickly become hundreds, and then looking for that exact title we reviewed back in 2015 would be a challenge! So here we have the complete list of all posts made by us. We hope this helps.

Oh, and by the way, these are in the reverse chronological order:

<section class="archive-post-list">

   {% for post in site.posts %}
      {% assign author = site.authors[post.author] %}
      {% assign currentDate = post.date | date: "%Y" %}
       {% if currentDate != myDate %}
          {% unless forloop.first %}</ul>{% endunless %}
          <p>{{ currentDate }}</p>
          <ul>
          {% assign myDate = currentDate %}
      {% endif %}
      <li><a href="{{ post.url }}"><span>{{ post.date | date: "%B %-d, %Y" }}</span> - {{ post.title }}</a> by <a href="/author/{{ author.name }}">{{ author.displayname }}</a></li>
      {% if forloop.last %}</ul>{% endif %}
   {% endfor %}

</section>
