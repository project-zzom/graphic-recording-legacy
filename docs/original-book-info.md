---
layout: default
---

## 원서 정보

> {{ site.data.books.original.description.long }}

* 도서명: [{{ site.data.books.original.title.main }}]()
* 저자: {% for author in site.data.authors-original %}[{{ author.name }}]({{ author.profile }}){% unless forloop.last%}, {% endunless %}{% endfor %}
* 출판사: [{{ site.data.books.original.publisher.name }}]({{ site.data.books.original.publisher.url }})

{% if site.data.books.original.cover.url %}
<img class="cover" src="{{ site.data.books.original.cover.url | relative_url }}" alt="Cover" class="cover-middle"/> 
{% endif %}

***

## 판매처

{% for store in site.data.stores-original %}<a href="{{ store.link }}" target="{{ store.target }}">{{ store.name }}</a>{% unless forloop.last%} / {% endunless %}{% endfor %}