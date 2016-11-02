# fontAwesome-SCSS
[![GitHub version](https://badge.fury.io/gh/reskwer%2FfontAwesome-SCSS.svg)](https://badge.fury.io/gh/reskwer%2FfontAwesome-SCSS) [![npm version](https://badge.fury.io/js/fontawesome-scss.svg)](https://badge.fury.io/js/fontawesome-scss)

### Почему fontAwesome-SCSS ?
1. Не подключаете шрифты. экономия `http` запроса.
2. Не выгружаете `150 kb` ради 1 иконки.
3. Все иконки в `SGV`
4. Не теряет качество при отключеном сглаживание шрифтов.
5. Не кривыит иконки если по каким-то причинам файл шрифтов не выгрузился или выгрузился с ошибками.
6. Все иконки из версии `4.7`

## Install
Скачайте архив и подлючите файл `fontAwesome.scss` в ваш проект.    

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

## npm 
`npm i fontawesome-scss --save-dev`

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

