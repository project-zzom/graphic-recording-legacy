---
layout: default-jp
---

## 원서 정보

> {{ site.data.books.jp.description.long }}

* 도서명: {{ site.data.books.jp.title.main }}
* 부제: {{ site.data.books.jp.title.sub }}
* 저자: {% for author in site.data.authors-jp %}<a href="{{ author.profile }}" target="_blank">{{ author.name }}</a>{% unless forloop.last%}, {% endunless %}{% endfor %}
* 출판사: <a href="{{ site.data.books.jp.publisher.url }}" target="_blank">{{ site.data.books.jp.publisher.name }}</a>

***

## 판매처

{% for store in site.data.stores-jp %}<a href="{{ store.link }}" target="{{ store.target }}">{{ store.name }}</a>{% unless forloop.last%} / {% endunless %}{% endfor %}