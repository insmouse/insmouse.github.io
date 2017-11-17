---
layout: post
comments: true
test_text: TESTTEXT (variabel) I BLOG_POSTS
title:  "Blogginlägg"
date:   2017-11-07 09:13:06 -0600
categories: jekyll update
permalink: /blog/
fruit:
  - äpple
  - kaviar
  - mellanslag
merfrukt:
  - name: apple
    cost: $1
    color: red
  - name: banana
    cost: $2
    color: yellow
  - name: orange
    cost: $1.50
    color: orange
---


detta är blog_posts

<section>
  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        {% assign date_format = site.minima.date_format | default: "%b %-d, %Y" %}
        <span class="post-meta">{{ post.date | date: date_format }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
        </h2>
      </li>
    {% endfor %}
  </ul>
</section>
