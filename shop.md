---
layout: page
title: Shop
permalink: /shop.html

---
<ul class="products">
{% for product in site.products %}
<li>
    <img src="{{ product.thumbnail }}" alt="{{ product.title }}"/>
    <h3><a href="{{ product.url }}">{{ product.title }}</a></h3>
    <span class="price">{{ product.price | format_as_money }}</span>
</li>
{% endfor %}
</ul>
