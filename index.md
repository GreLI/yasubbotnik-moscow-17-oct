---

layout: default
title: Приручаем SVG

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

## Поддержка

* IE 9+ (фильтры IE 10+, но баги масштабирования)
* Firefox 4+ (раньше только object, баг с размытием)
* iOS
* Android 3+ (полноценно 4.4+)

## Примитивы

![placeholder](pictures/primitives.svg){:.right-image}

~~~ markup
<rect x="0" y="0" width="100" height="60"
    rx="15" fill="skyblue"/>

<circle cx="150" cy="40" r="40" fill="pink"/>

<ellipse cx="120" cy="100" rx="100" ry="40"
    transform="rotate(10)" fill="peachpuff"/>

<line x1="15" y1="210" x2="255" y2="180"
    stroke="silver"/>

<polyline points="30,270 80,230 150,260 220,220
    290,230" stroke="tan" fill="none"/>

<polygon points="290,80 265,123.2 215,123.2 190,80 214.96,36.8 265,36.8"
    fill="lightgreen"/>
~~~
{:.top-code}

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

## Начинаем рисовать

![Размытый прямоугольник](pictures/blurry-rect.png){:.right-image}

~~~ markup
<svg xmlns="http://www.w3.org/2000/svg"
     width="50" height="50"
     viewBox="0 0 50 50">
  <rect x="5" y="5" width="40" height="40"
        rx="5" stroke-width="1"
        stroke="black" fill="none"/>
</svg>
~~~
{:.top-code}

## path

## Текст

* Пишем текст
* Графические эффекты

## Группировка и переиспользование

## Иконки

## Маски

## Трансформации

## viewBox

## Маски

## Фильтры

## Анимация

* SMIL
* Javascript
* CSS анимации
* Будущее: Web Animations

## Методы вставки

* Object
* Iframe
* \<img\>
* CSS
* HTML5

## Object/Iframe

* Можно вставлять ссылки на внешние ресурсы
* Можно вставлять скрипты
* Доступно для JS страницы
* Трудно стилизовать, надо задавать размеры
* Не наследуются стили страницы

## \<img\>

* Нельзя вставлять ссылки на внешние ресурсы
* Нельзя вставлять скрипты
* Недоступно для JS страницы
* Браузер применит размеры картинки, если они есть
* Не наследуются стили страницы

## CSS

* Нельзя вставлять ссылки на внешние ресурсы
* Нельзя вставлять скрипты
* Недоступно для JS страницы
* Браузер применит размеры картинки, если они есть
* Не наследуются стили страницы
* Имеют почти все преимущества картинок в CSS (но есть баги)

## HTML5

* Можно вставлять ссылки на внешние ресурсы
* Можно  вставлять скрипты
* Единое глобальное пространство JS со страницей
* Браузер применит размеры картинки, если они есть
* Стили страницы наследуются.
* Можно переиспользовать элементы других SVG.

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
