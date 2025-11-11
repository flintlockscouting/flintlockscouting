---

layout: page
title: Scouting Activities
parent: Scouting Resources

---

Flintlock Favorite Scout Activities

See the Flintlock Guide: https://docs.google.com/document/d/1Ue8dZPevttFIrPBNMzinczP6kQIK7bwGeuAnEAcHRAk/edit?tab=t.0#heading=h.1dul3wpirolf

<ul>
{% for activity in site.activities %}
<li>
    <a href="{{ site.baseurl }}/{{ activity.url }}">
        {{ activity.name }}
    </a>
</li>
{% endfor %}
</ul>
