---

layout: page
title: Scouting Activities
parent: Scouting Resources

---

Flintlock Favorite Scout Activities

<ul>
{% for activity in site.activities %}
<li>
    <a href="{{ site.baseurl }}/{{ activity.url }}">
        {{ activity.name }}
    </a>
</li>
{% endfor %}
</ul>