---
layout: homepage.html
---

Podcast about games and game development.

We discuss game development, design and disect games we have played recently (while not really taking ourselves too seriously). We also talk about our own projects - past, present and future.

<ul>
{%- for episode in collections.episode -%}
  <li>
    <a href="{{ episode.url }}">
      Episode {{ forloop.index }}: {{ episode.data.title }}
    </a>
    <p>{{ episode.data.description }}</p>
  </li>
{%- endfor -%}
</ul>
