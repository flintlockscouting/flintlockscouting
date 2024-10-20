---

layout: page
title: Scouting Activities
parent: Scouting Resources

---

Flintlock Favorite Scout Activities

<ul>
{% for song in site.activities %}
<li>
    <a href="{{ activites.url }}">
        {{ activities.name }}
    </a>
</li>
{% endfor %}
</ul>