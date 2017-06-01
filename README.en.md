# fontAwesome-SCSS
[![GitHub version](https://badge.fury.io/gh/reskwer%2FfontAwesome-SCSS.svg)](https://badge.fury.io/gh/reskwer%2FfontAwesome-SCSS) [![npm version](https://badge.fury.io/js/fontawesome-scss.svg)](https://badge.fury.io/js/fontawesome-scss)

*Прочтите это на русском языке: [Russian](README.md)

### fontAwesome-SCSS ?
1. You don't have to load fonts which will eliminate an `http` request.
2. You don't need to download `150 kb` for 1 icon.
3. All icons `inline SGV` in CSS. Clean html
4. Don't loose quality when disabling font smoothing.
5. Don't askew icons if for some reason the font file wasn't loaded or loaded with errors.
6. All icons from version `4.7`

## Install
`npm i fontawesome-scss --save-dev`

or just simply add `fontAwesome.scss` to your project.

### Syntax
```scss
@include fa($icon-name, color, size)
```
**icon-name** - Name of the icon prepended by `$`, for example: `$fa-user`.
**color** - any value supported by `css`, hex, rgba, css variables.
**size** - any value supported by `css`
*You could skip any of the arguments*
### Example
Red color icon, 18px
```scss
.icon-user{
    @include fa($fa-user, red ,18px);
}
```
[![GitHub version](https://github.com/reskwer/fontAwesome-SCSS/blob/master/intro.gif?raw=true)      

CSS result
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
If you want to save time, here is sublime snippet.

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
fontawesome-scss is a teamwork of  
[reskwer](https://github.com/reskwer) and [sokoliurii](https://github.com/sokoliurii)
