## 번역서 정보

> {{ site.data.books.ko.description.long }}

* 도서명: {{ site.data.books.ko.title.main }}
* 부제: {{ site.data.books.ko.title.sub }}
* 번역자: {% for author in site.data.authors-ko %}<a href="{{ author.profile }}" target="_blank">{{ author.name }}</a>{% unless forloop.last%}, {% endunless %}{% endfor %}
* 출판사: <a href="{{ site.data.books.ko.publisher.url }}" target="_blank">{{ site.data.books.ko.publisher.name }}</a>
* 관련 자료: <a href="{{ site.url }}{{ site.baseurl }}/errata.html" target="_self">정오표</a> | 
<a href="{{ site.url }}{{ site.baseurl }}/downloads/visual-library.zip" target="_blank">다운로드</a>

## 판매처

* <a href="https://book.naver.com/bookdb/book_detail.nhn?bid=20916537" target="_blank">네이버 책</a>

<!--
{% for store in site.data.stores-ko %}<a href="{{ store.link }}" target="{{ store.target }}">{{ store.name }}</a>{% unless forloop.last%} / {% endunless %}{% endfor %} -->
