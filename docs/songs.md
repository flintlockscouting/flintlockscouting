---

layout: page
title: Scouting Songs
parent: Scouting Resources

---

Flintlock Favorite Scout Songs

<ul>
{% for song in site.songs %}
<li>
    <a href="{{ site.baseurl }}/{{ song.url }}">
        {{ song.name }}
    </a>
</li>
{% endfor %}
</ul>