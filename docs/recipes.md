---

layout: page
title: Camping Recipes
parent: Scouting Resources

---

Flintlock Favorite Camping Recipes 

<ul>
{% for recipe in site.recipes %}
<li>
    <a href="{{ site.baseurl }}/{{ recipe.url }}">
        {{ recipe.name }}
    </a>
</li>
{% endfor %}
</ul>