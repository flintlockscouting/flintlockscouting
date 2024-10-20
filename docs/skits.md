---

layout: page
title: Campfire Skits
parent: Scouting Resources

---

Flintlock Favorite Campfire Skits

<ul>
{% for skit in site.skits %}
<li>
    <a href="{{ site.baseurl }}/{{ skit.url }}">
        {{ skit.name }}
    </a>
</li>
{% endfor %}
</ul>