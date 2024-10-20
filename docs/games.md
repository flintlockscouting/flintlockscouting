---

layout: page
title: Games
parent: Scouting Resources

---

Flintlock Favorite Games

<ul>
{% for game in site.games %}
<li>
    <a href="{{ game.url }}">
        {{ game.name }}
    </a>
</li>
{% endfor %}
</ul>