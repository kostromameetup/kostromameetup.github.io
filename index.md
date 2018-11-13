---
layout: page
title: 24 ноября 2018
excerpt:
comments: true
---

[**Регистрируйся**][register] и приходи – мы ждем тебя!
	

Доклады
-------

<ul class="post-list">
{% for post in site.categories.talks %}
  {% if post.author %}
    {% capture authorslist %}
      {% for a in post.author %}
        {% assign author = site.data.authors[a] %}
        {% if author %} {{ author.name }}{% if author.company %}, {{ author.company }}{% endif %}{% endif %}{% unless forloop.last %};{% endunless %}
      {% endfor %}
    {% endcapture %}
  {% endif %}
  {% if post.announce %}
  <li><a href="{{ site.url }}{{ post.url }}"><b>{{ post.title }}</b><br/>{{ authorslist }}</a></li>
  {% endif %}
{% endfor %}
</ul>

Когда
-----

Итак, __24 ноября в 16:00__ состоится встреча программистов в рамках KsTF – 2018. На все доклады  отведено  3  часа. Между  выступлениями  запланирован  кофе-брейк, чтобы  вы  могли перекусить. Для первых 30-ти зарегистрировавшихся after-party за счет компании!

Дата: 24/11/2018, суббота.

Время: с 16.00 до 19.00.

__Вход – free.__


Где
---

Встреча пройдет по адресу: г. Кострома, ул. Чайковского, 9 Б. Бизнес-центр «Luxuria», большой конференц-зал.

Ближайшая остановка общественного транспорта указана на карте зеленым цветом.

Места для парковки автомобилей указаны на карте красным цветом.

Контактные телефоны:

__+7 (950) 247-33-68 Егор__

__+7 (909) 249-11-00 Мария__


<script type="text/javascript" charset="utf-8" async src="https://api-maps.yandex.ru/services/constructor/1.0/js/?um=constructor%3A813d2bb074f64db25b4f9622e799ee9a9b139d077b2e54d06aa249a8825fdeef&amp;width=606&amp;height=556&amp;lang=ru_RU&amp;scroll=true"></script>


<!--
<ul class="post-list">
{% for post in site.posts limit:10 %}
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span></a></article></li>
{% endfor %}
</ul>
-->

[register]: /register/
[place]: http://www.conferencelux.ru/index.aspx
[tensor]: http://tensor.ru/
[speakers]: /speakers/
