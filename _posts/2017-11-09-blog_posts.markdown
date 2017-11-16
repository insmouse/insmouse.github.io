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



<section>

    <ul>
      {% for grej in page.fruit %}
        <li>{{ grej }} är inte gott</li>

      {% endfor %}
    </ul>


    <ul>
      {% for apa in page.merfrukt %}
        <li>{{ apa.name }}, cost: {{ apa.cost }}, color: {{ apa.color }}</li>
      {% endfor %}
    </ul>


</section>


# Blogginlägg

## Här samlar jag alla mina blogginlägg.

# {{ page.test_text }}
Denna variabel påverkas av MD-rubrikformat!

{% include youtube.html youtube_id="YIiHiMXOeYU" %}

---

* (Länk 1)
* (Länk 2)
* (Länk 3)

---

SÅ HÄR SKRIVER MAN TYDLIGEN MARKDOWN

# Heading

## Sub-heading

### Another deeper heading

Paragraphs are separated
by a blank line.

Two spaces at the end of a line leave a
line break.

Text attributes _italic_, *italic*, __bold__, **bold**, `monospace`.

Horizontal rule:

---

Bullet list:

  * apples
  * oranges
  * pears

Numbered list:

  1. apples
  2. oranges
  3. pears

A [link](http://example.com).

---

[*Tillbaka till startsidan*] [post-1]

[post-1]: welcome-to-jekyll.html
