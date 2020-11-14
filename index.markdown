---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: homepage
---

<div class="index_table">

{% for i in (0..24) %}
<div class="index_day">
 {% assign ingredient = site.data.ingredients.ingredients[i] %}
    <a href="./pages/{{ ingredient.name | downcase | replace: " ", "_" }}">
      {{ i | plus: "1" }}
    </a>
</div>
{% endfor %}
</div>