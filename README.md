# fontAwesome-SCSS
[![GitHub version](https://badge.fury.io/gh/reskwer%2FfontAwesome-SCSS.svg)](https://badge.fury.io/gh/reskwer%2FfontAwesome-SCSS) [![npm version](https://badge.fury.io/js/fontawesome-scss.svg)](https://badge.fury.io/js/fontawesome-scss)
## Install
1. Скачайте миксин.
2. С папки "fonts" скопируйте шрифты в папку вашего проекта.
3. Подключите fontAwesome.scss , `@import "fontAwesome.scss";`
4. В файле `fontAwesome.scss`, переменной `$folderFonts` задайте путь к папке со шрифтами fontAwesome. ВНИМАНИЕ: путь нужно задавать так - как в css, не с корня сайта, а с к корня папки css.

Пример
```scss
span {
    @include fa($fa-user)
}
```
Так же доступны ключи для быстрой стилизации `:before или :after`, `font-size`, `color`, `margin`, `vertical-align` в качестве ключей можно использовать вседоступные CSS единицы

Пример
```scss
span {
    @include fa($fa-user, before, 18px, #ccc, 0 5px, middle)
}
```
Данный код будет скомпилирован в:
```css
.span:after {
    content: "";
    display: inline-block;
    font-size: 18px;
    line-height: 1;
    font-family: FontAwesome;
    color: #ccc;
}
```

Документация написана на быструю руку, со временем будет будет дополнятся.