---
layout: page
title: Shop
permalink: /shop/
---
<ul class="products">
{% for product in site.products %}
<li>
    <img src="{{ product.image1 }}" alt="{{ product.title }}"/>
    <h4><a href="{{ product.url }}">{{ product.title }}</a></h4>
    <span class="price">Rp. {{ product.price | format_as_money }},-</span>
</li>
{% endfor %}
</ul>
