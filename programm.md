---
layout: default
---

{% assign pages = (site.pages | sort: "page-category" | reverse | where_exp: "page", "page.page-category contains 'session'")  %}
{% assign pages1 = (pages | where: "room", "15.04") %}
{% assign pages2 = (pages | where: "room", "15.05") %}
{% assign pages3 = (pages | where: "room", "15.06") %}
{% assign pages4 = (pages | where: "room", "10.02") %}
{% assign pages5 = (pages | where: "room", "10.07") %}
{% assign sortedPages = pages1 %}
{% for page in pages2 %}
  {% assign sortedPages = sortedPages | push: page %}
{% endfor %}
{% for page in pages3 %}
  {% assign sortedPages = sortedPages | push: page %}
{% endfor %}
{% for page in pages4 %}
  {% assign sortedPages = sortedPages | push: page %}
{% endfor %}
{% for page in pages5 %}
  {% assign sortedPages = sortedPages | push: page %}
{% endfor %}

# Programm

<div class="program">
<h2>08:30 - 09:15
<p>Check-In / Kaffee, Getränke und kleine Snacks im 15. Stock</p>
</h2>

<h2>09:15 - 9:45 Keynote</h2>

To be announced soon ...

<div class="card-deck">
{% assign slotPages = (sortedPages | where: "slot", "S0900") %}
{% for page in slotPages %}
        {% capture title %}{{ page.title }}{% endcapture %}
        {% capture speaker %}{{ page.speaker }}{% endcapture %}
        {% capture speaker-id %}{{ page.speaker-id }}{% endcapture %}
        {% capture room %}{{ page.room }}{% endcapture %}
        {% capture url %}{{ page.url }}{% endcapture %}
        {% capture page-category %}{{ page.page-category }}{% endcapture %}
        {% include card.html title=title speaker=speaker speaker-id=speaker-id room=room url=url page-category=page-category  %}
{% endfor %}
</div>

<h2>09:45 - 09:55
<p>Kaffee und Getränke im 15. Stock</p>
</h2>

<h2>09:55 bis 10:45</h2>

To be announced soon ...

<div class="card-deck">
{% assign slotPages = (sortedPages | where: "slot", "S1000") %}
{% for page in slotPages %}
        {% capture title %}{{ page.title }}{% endcapture %}
        {% capture speaker %}{{ page.speaker }}{% endcapture %}
        {% capture speaker-id %}{{ page.speaker-id }}{% endcapture %}
        {% capture room %}{{ page.room }}{% endcapture %}
        {% capture url %}{{ page.url }}{% endcapture %}
        {% capture page-category %}{{ page.page-category }}{% endcapture %}
        {% include card.html title=title speaker=speaker speaker-id=speaker-id room=room url=url page-category=page-category  %}
{% endfor %}
</div>

<h2>10:45 - 11:10
<p>Kaffee und Getränke im 15. Stock</p>
</h2>

<h2>11:10 - 12:00</h2>

To be announced soon ...

<div class="card-deck">
{% assign slotPages = (sortedPages | where: "slot", "S1100") %}
{% for page in slotPages %}
        {% capture title %}{{ page.title }}{% endcapture %}
        {% capture speaker %}{{ page.speaker }}{% endcapture %}
        {% capture speaker-id %}{{ page.speaker-id }}{% endcapture %}
        {% capture room %}{{ page.room }}{% endcapture %}
        {% capture url %}{{ page.url }}{% endcapture %}
        {% capture page-category %}{{ page.page-category }}{% endcapture %}
        {% include card.html title=title speaker=speaker speaker-id=speaker-id room=room url=url page-category=page-category  %}
{% endfor %}
</div>

<h2>12:00 - 13:00 Mittagspause
<p>Warmes Mittagessen im 15. Stock</p>
</h2>

<h2>13:00 - 13:50</h2>

To be announced soon ...

<div class="card-deck">
{% assign slotPages = (sortedPages | where: "slot", "S1300") %}
{% for page in slotPages %}
        {% capture title %}{{ page.title }}{% endcapture %}
        {% capture speaker %}{{ page.speaker }}{% endcapture %}
        {% capture speaker-id %}{{ page.speaker-id }}{% endcapture %}
        {% capture room %}{{ page.room }}{% endcapture %}
        {% capture url %}{{ page.url }}{% endcapture %}
        {% capture page-category %}{{ page.page-category }}{% endcapture %}
        {% include card.html title=title speaker=speaker speaker-id=speaker-id room=room url=url page-category=page-category  %}
{% endfor %}
</div>

<h2>13:50 - 14:00
<p>Kaffee, Getränke und Kuchen im 15. Stock</p>
</h2>

<h2>14:00 - 14:50</h2>

To be announced soon ...

<div class="card-deck">
{% assign slotPages = (sortedPages | where: "slot", "S1400") %}
{% for page in slotPages %}
        {% capture title %}{{ page.title }}{% endcapture %}
        {% capture speaker %}{{ page.speaker }}{% endcapture %}
        {% capture speaker-id %}{{ page.speaker-id }}{% endcapture %}
        {% capture room %}{{ page.room }}{% endcapture %}
        {% capture url %}{{ page.url }}{% endcapture %}
        {% capture page-category %}{{ page.page-category }}{% endcapture %}
        {% include card.html title=title speaker=speaker speaker-id=speaker-id room=room url=url page-category=page-category  %}
{% endfor %}
</div>

<h2>14:50 - 15:10
<p>Kaffee, Getränke und Kuchen im 15. Stock</p>
</h2>

<h2>15:10 - 16:00</h2>

To be announced soon ...

<div class="card-deck">
{% assign slotPages = (sortedPages | where: "slot", "S1500") %}
{% for page in slotPages %}
        {% capture title %}{{ page.title }}{% endcapture %}
        {% capture speaker %}{{ page.speaker }}{% endcapture %}
        {% capture speaker-id %}{{ page.speaker-id }}{% endcapture %}
        {% capture room %}{{ page.room }}{% endcapture %}
        {% capture url %}{{ page.url }}{% endcapture %}
        {% capture page-category %}{{ page.page-category }}{% endcapture %}
        {% include card.html title=title speaker=speaker speaker-id=speaker-id room=room url=url page-category=page-category  %}
{% endfor %}
</div>

<h2>16:00 - 16:05
<p>Pause</p>
</h2>

<h2>16:05 - 16:15 Abschluss des GAB 2018</h2>

To be announced soon ...

<div class="card-deck">
{% assign slotPages = (sortedPages | where: "slot", "S1600") %}
{% for page in slotPages %}
        {% capture title %}{{ page.title }}{% endcapture %}
        {% capture speaker %}{{ page.speaker }}{% endcapture %}
        {% capture speaker-id %}{{ page.speaker-id }}{% endcapture %}
        {% capture room %}{{ page.room }}{% endcapture %}
        {% capture url %}{{ page.url }}{% endcapture %}
        {% capture page-category %}{{ page.page-category }}{% endcapture %}
        {% include card.html title=title speaker=speaker speaker-id=speaker-id room=room url=url page-category=page-category  %}
{% endfor %}
</div>
</div>