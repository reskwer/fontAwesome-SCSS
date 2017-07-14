# fontAwesome-SCSS
[![GitHub version](https://badge.fury.io/gh/reskwer%2FfontAwesome-SCSS.svg)](https://badge.fury.io/gh/reskwer%2FfontAwesome-SCSS) [![npm version](https://badge.fury.io/js/fontawesome-scss.svg)](https://badge.fury.io/js/fontawesome-scss)

*Read this in English: [English](README.en.md)

### fontAwesome-SCSS ?
1. Не нужно подключать шрифты. Экономия `http` запроса.
2. Не выгружаете `150 kb` ради 1 иконки.
3. Все иконки `inline SGV` в CSS. Чистый html
4. Не теряет качество при отключённом сглаживание шрифтов.
5. Не кривыит иконки если по каким-то причинам файл шрифтов не выгрузился или выгрузился с ошибками.
6. Все иконки из версии `4.7`

## Install
`npm i fontawesome-scss --save-dev`

или просто закиньте `fontAwesome.scss` в ваш проект.

### Синтаксис
```scss
@include fa($имя-иконки, цвет, размер)
```
**Имя** - Имена иконок указываются и приставкой `$`, пример: `$fa-user`.
**Цвет** - любое значение поддерживаемое `css`, hex, rgba, css переменные.
**Размер** - любое значение поддерживаемое `css`
*Любое значение можно пропустить*
### Пример
Иконка красного цвета, 18px
```scss
.icon-user{
    @include fa($fa-user, red ,18px);
}
```
[![GitHub version](https://github.com/reskwer/fontAwesome-SCSS/blob/master/intro.gif?raw=true)      

CSS на выходе
```css
.text:before {
    content: '\00A0';
    display: inline-block;
    line-height: 44px;
    width: 44px;
    height: 44px;
    background-image: url(data:image/svg+xml utf8, <svg xmlns="http://www.w3.org/2000/svg" x="0px" y="6.5-37.5,271.5-112.5S1876,22,1876-84 S1838.5-280.5,1763.5-355.5z"/></svg>);
}
```

## Sublime
Для тех кто ценит свое время, sublime сниппет.
```xml
<snippet>
	<content><![CDATA[
@include fa (\$${1:name});
]]></content>
	<tabTrigger>fa</tabTrigger>
	<scope>source.scss</scope>
</snippet>
```

## copyright
fontawesome-scss - является совместной работой 
[reskwer](https://github.com/reskwer) и [sokoliurii](https://github.com/sokoliurii)
