---

layout: default

---

# Яндекс

## **{{ site.presentation.title }}** {#cover}

<div class="s">
    <div class="service">{{ site.presentation.service }}</div>
</div>

{% if site.presentation.nda %}
<div class="nda"></div>
{% endif %}

<div class="info">
  <p class="author">{{ site.author.name }}, <br/> {{ site.author.position }}</p>
</div>

## Введение
{:.section}

### WTF is SVG

## SVG — Scalable Vector Graphics

### Векторная графика

* Масштабируется
* Хорошо смотрится на любых DPI
* XML-документ (прост почти как HTML)

## Пример кода: логотип SVG

~~~ markup
<svg xmlns="http://www.w3.org/2000/svg"
     xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 300 300">
  <title>SVG Logo</title>
  <desc>Designed for the SVG Logo Contest in 2006 b  Harvey Rayner, and
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
