---
layout: post
title:  "Robots.txt och humans.txt"
date:   2017-11-07 09:13:06 -0600
categories: examination-1
comments: true
---

### Vad är robots.txt och hur har du konfigurerat den för din sajt?

<!--more-->

Robots.txt är en textfil som ger instruktioner till robotar/sökmotorer om hur de ska genomsöka den aktuella sajten. Exempelvis kan man exkludera vissa kataloger, eller vissa sökmotorer. Det går också att ge sökmotorerna andra instruktioner, som att hjälpa dem genom att peka dem till sajtens sitemap.

Så här ser min robots.txt-fil ut:

User-agent: *
Disallow: /

"User-agent: *" betyder "alla robotar", och "Disallow: /" att hela sajten exkluderas. Detta innebär att alla sökmotorer i teorin förhindras från att (eller snarare ombeds att inte) gå igenom innehållet. Jag valde att stänga ute sökmotorer på detta vis eftersom det här är en sajt med övningsuppgifter och liknande som jag inte vill skylta med utanför denna kurs.

### Vad är humans.txt och hur har du konfigurerat den för din sajt?

Medan robots.txt är till för just "robotar" så riktar sig humans.txt till människor. I denna textfil kan man, om man vill, berätta om sitt projekt och de som varit inblandade i utvecklingen. Exempelvis kan man räkna upp utvecklarna och deras kontaktuppgifter, ange sajtens språk och berätta vilka programvaror som använts.

I min humans.txt-fil har jag angett mitt namn, min studentmail, mitt Github-namn, min hemstad, datum för sajtens senaste uppdatering, programvaror jag använt, samt sajtens språk.
