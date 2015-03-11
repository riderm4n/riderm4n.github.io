---
layout: page
title: Shop
permalink: /shop/
---
<ul class="products small-block-grid-1 medium-block-grid-2">
{% for product in site.products %}
<li>
    <a href="{{ product.url }}">
        <img src="{{ product.image1 }}" alt="{{ product.title }}"/>
        <h4>{{ product.title }}</h4>
    </a>
    <span class="price">Rp. {{ product.price | format_as_money }},-</span>
</li>
{% endfor %}
</ul>
