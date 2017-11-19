---
layout: post
title:  "Kommentarer och Open Graph"
date:   2017-11-18 09:13:06 -0600
categories: examination-1
comments: true
---

### Hur implementerade du kommentarer i dina blogginlägg?

<!--more-->

Jag använde mig av tredjepartslösningen Disqus. För att ordna Disqus-stödet på min sajt skapade jag ett konto samt följde installationsguiden för Jekyll på disqus.com. I de inlägg som ska ha kommentarer har jag angett "comments: true" i front matter. I koden för layouten post.html finns "if page.comments"-taggar, som gör att kommentarer bara laddas på sidor som har "comments: true" i sin front matter.

### Vad är Open Graph och hur använder du det?

Open Graph är en standard som gör att sociala medie-plattformar som Facebook kan förhandsvisa en sidas innehåll på ett sätt som sidans ägare själv kan skräddarsy. Med hjälp av en uppsättning taggar i den aktuella sidans head kan man skicka med ett valfritt antal egenskaper till den plattform där sidan delas.

Genom att använda koden nedan har jag valt att skicka med den aktuella sidans titel, typen av innehåll (webbplats), URL samt – eftersom dessa inlägg inte behöver några egna bilder – min profilbild.

{% highlight html %}

  <meta property="og:title" content="{{ page.title }}" />
  <meta property="og:type" content="website" />
  <meta property="og:url" content="{% capture url_path %}{{site.url}}{{page.url}}{% endcapture %}" />
  <meta property="og:image" content="/img/avatar.jpg" />

{% endhighlight %}
