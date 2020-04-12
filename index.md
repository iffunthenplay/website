---
layout: homepage.html
---

Podcast about games.

<ul>
{%- for episode in collections.episode -%}
  <li>
    <a href="{{ episode.url }}">
      Episode {{ forloop.index }}: {{ episode.data.title }}
    </a>
    <p>{{ episode.description }}</p>
  </li>
{%- endfor -%}
</ul>
