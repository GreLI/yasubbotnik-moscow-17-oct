---

layout: default
title: SVG в вебе

---

# Яндекс

## **{{ site.presentation.title }}** {#cover}

<!-- <div class="s">
    <div class="service">{{ site.presentation.service }}</div>
</div> -->

{% if site.presentation.nda %}
<div class="nda"></div>
{% endif %}

<div class="info">
  <p class="author">{{ site.author.name }}, <br/> {{ site.author.position }}</p>
</div>

## <sup>*</sup>Что такое SVG
{:.section}

### WTF is SVG

## SVG — Scalable Vector Graphics

### Производный формат VML (Microsoft) и PGML (разработан из Adobe PostScript)

* Масштабируемая
* Чёткая на любых DPI
* XML-документ
* Можно редактировать в текстовом редакторе
* Может включать растровые изображения, ссылки, стили, скрипты

## Как выглядит SVG
{:.section}

### Пример кода

## Пример кода: логотип SVG

~~~ markup
<svg xmlns="http://www.w3.org/2000/svg"
     xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 300 300">
  <title>SVG Logo</title>
  <desc>Designed for the SVG Logo Contest in 2006 by Harvey Rayner, and
    adopted by W3C in 2009. It is available under the Creative Commons license
    for those who have an SVG product or who are using SVG on their site.</desc>
  <g stroke-width="38" stroke="#000">
    <g id="b" transform="translate(150 150)">
      <path id="a" fill="#ffb13b" d="M-84.15,-15.85
        a22.417,22.417 0 1 0 0,31.7 h168.3 a22.417,22.417 0 1 0 0,-31.7z"/>
      <use xlink:href="#a" transform="rotate(45)"/>
      <use xlink:href="#a" transform="rotate(90)"/>
      <use xlink:href="#a" transform="rotate(135)"/>
    </g>
  </g>
  <use xlink:href="#b"/>
</svg>
~~~

## Как выглядит в браузере: логотип SVG
{:.center}

![](pictures/svg-logo.svg){:.horizontal-big}

## Примитивы

### Вводный текст (первый уровень текста)
![placeholder](pictures/primitives.svg){:.right-image}

~~~ markup
<rect x="0" y="0" width="100" height="60" rx="15" fill="skyblue"/>
<circle cx="150" cy="40" r="40" fill="pink"/>
<ellipse cx="120" cy="100" rx="100" ry="40" transform="rotate(10)" fill="peachpuff"/>
<line x1="15" y1="210" x2="255" y2="180" stroke="silver"/>
<polyline points="30,270 80,230 150,260 220,220 290,230" stroke="skyblue"/>
<polygon points="150,75 258,137.5 258,262.5 150,325 42,262.6 42,137.5" fill="lightgreen" transform="translate(180 0) scale(.4) rotate(90 150 200)"/>
~~~

Текст
{:.note}

## &nbsp;
{:.with-big-quote}
> Цитата

Текст
{:.note}

## Пример подсветки кода
{:.code-with-text}

Вводный текст

~~~ javascript
var jar,
    rstoreNames = /[^\w]/g,
    storageInfo = window.storageInfo || window.webkitStorageInfo,
    toString = "".toString;

jar = this.jar = function( name, storage ) {
    return new jar.fn.init( name, storage );
};
~~~

## &nbsp;
{:.big-code}

~~~ javascript
!function() {
    var jar,
        rstoreNames = /[^\w]/g,
        storageInfo = window.storageInfo || window.webkitStorageInfo,
        toString = "".toString;

    jar = this.jar = function( name, storage ) {
        return new jar.fn.init( name, storage );
    };

    jar.storages = [];
    jar.instances = {};
    jar.prefixes = {
        storageInfo: storageInfo
    };
}.call( window );
~~~

## LaTeX

Библиотека для латекса довольно тяжелая, а нужна она в редких случаях.
Поэтому она не включена в репу, ее нужно либо установить через bower либо иметь интернет.

When $a \ne 0$, there are two solutions to \(ax^2 + bx + c = 0\) and they are
$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

## Заголовок
{:.images}

![](pictures/horizontal-placeholder.png)
*Текст*

![](pictures/horizontal-placeholder.png)
*Текст*

![](pictures/horizontal-placeholder.png)
*Текст*

## Заголовок
{:.images .two}

![](pictures/horizontal-middle-placeholder.png)
*Текст*

![](pictures/horizontal-middle-placeholder.png)
*Текст*

## Заголовок
{:.center}

![](pictures/horizontal-big-placeholder.png){:.tmp}

## **![](pictures/cover-placeholder.png)**

## ![](pictures/horizontal-cover-placeholder.png)
{:.cover}

## Таблица

|  Locavore      | Umami       | Helvetica | Vegan     |
+----------------|-------------|-----------|-----------+
| Fingerstache   | Kale        | Chips     | Keytar    |
| Sriracha       | Gluten-free | Ennui     | Keffiyeh  |
| Thundercats    | Jean        | Shorts    | Biodiesel |
| Terry          | Richardson  | Swag      | Blog      |
+----------------|-------------|-----------|-----------+


## Таблица с дополнительным полем

{:.with-additional-line}
|  Locavore      | Umami       | Helvetica | Vegan     |
+----------------|-------------|-----------|-----------+
| Fingerstache   | Kale        | Chips     | Keytar    |
| Sriracha       | Gluten-free | Ennui     | Keffiyeh  |
| Thundercats    | Jean        | Shorts    | Biodiesel |
| Terry          | Richardson  | Swag      | Blog      |
+----------------|-------------|-----------|-----------+
| Terry          | Richardson  | Swag      | Blog      |

## **Контакты** {#contacts}

<div class="info">
<p class="author">{{ site.author.name }}</p>
<p class="position">{{ site.author.position }}</p>

    <div class="contacts">
        <!-- <p class="contacts-left contacts-top phone">+7 (000) 000-00-00</p> -->
        <p class="contacts-left mail">lev.sun@yandex.ru</p>
        <p class="contacts-right contacts-top twitter">@ruGreLI</p>
        <!-- <p class="contacts-right contacts-bottom vk">vk</p> -->
        <!-- <p class="contacts-right facebook">facebook</p> -->
    </div>
</div>
