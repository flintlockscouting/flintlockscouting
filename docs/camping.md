---

layout: page
title: Camping Locations
parent: Scouting Resources

---

Flintlock Favorite Camping Locations

<ul>
{% for song in site.camping %}
<li>
    <a href="{{ camp.url }}">
        {{ camp.name }}
    </a>
</li>
{% endfor %}
</ul>