---
layout: homepage.html
---

It's a podcast about making games, by developers who sometimes finish what they set out to do!

We chat about programming, designing, and we break down the games we're playing and building.

Nothing is taken too seriously.

{% assign episodes = collections.episode | reverse %}

<ul class="episode-list">
{%- for episode in episodes -%}
  <li>
    <a href="{{ episode.url }}">
      Episode {{ episode.data.number }}: {{ episode.data.title }}
    </a>
    <p>{{ episode.data.description }}</p>
  </li>
{%- endfor -%}
</ul>
