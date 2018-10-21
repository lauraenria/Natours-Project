# Learning tips

* [CSS clip-path maker](https://bennettfeely.com/clippy/)

## Install NPM and Sass

* `node -v` (check your version)
* `npm init` (open json file for us) to create a packet of json file
* `npm install node-sass --save-dev`

example;
* npm install jquery
* npm unistall jquery --save

```javascript
"script": {
"compile:sass": "node-sass sass/main.scss css/style.css -w"
}
```
* `npm run compile:sass`

* `npm install live-server -g`
* live-server

## Bugs

* if `@import` doens't work properly but everything seems perfect remember to restart SASS

* Check classes correspondence between HTML and Css/Sass

[Check here my project!](https://xenodochial-ritchie-156b6b.netlify.com/)

tips:

```css
&:not(:last-child) {}
}

.col-1-of-2 {
    width: calc((100% - #{$gutter-vertical}) / 2);
    background-color: orange;
    float: left;

    &:not(:last-child) {
        margin-right: $gutter-horizontal;
    }
}

.col-1-of-3 {
    width: calc((100% - 2 * #{$gutter-vertical}) / 3);
    background-color: lightgreen;
    float: left;

    &:not(:last-child) {
        margin-right: $gutter-horizontal;
    }
}



/* select all the classes which start with col- */
[class^='col-'] {}


/* select any classes which contain with col- */

[class*='col-'] {}

/* select any classes which ends with col- */

[class$='col-'] {}

/* select all direct child */
& > * 

```

### CSS property to remember

* **outline**(shorthand): An outline is a line that is drawn around elements, outside the borders, to make the element "stand out".

* **outline-offset**: dds space between an outline and the edge or border of an element.

*  **perspective**: it must be set on the parent of the 3D-positioned child we want to give it some perspective

* **backface-visibility**: Hide and show the back face an element


### Emmet

```css

/* .nameclass + tab */
/* .test */
<div class="test"></div>

/* tag.nameclass + tab */
/* section.section-about */
<section class="section-about"></section>`

/* lorem + tab */
/* random text */

/* &rarr; */
<a href="#" class="btn-text">Learn more &rarr;</a>

/* defining the children of the composition class */
.composition>img.composition__photo

.composition>(img.composition__photo.composition_photo--p1)*3

<div class="composition">
    <img src="" alt="" class="composition__photo composition_photo--p1">
    <img src="" alt="" class="composition__photo composition_photo--p1">
    <img src="" alt="" class="composition__photo composition_photo--p1">
</div>

.row>.col-1-of-4.feature-box*4

<div class="row">
    <div class="col-1-of-4 feature-box"</div>
    <div class="col-1-of-4 feature-box"</div>
    <div class="col-1-of-4 feature-box"</div>
    <div class="col-1-of-4 feature-box"</div>
</div>


```

## Flexible images

Always to define the width of images with percentages if possible because in this way they will scale nicely with the viewport

## resources

* [loremipsum generator](https://loremipsum.io/)
* [codingheroes](http://codingheroes.io/resources/)
* [HTML Entity Reference by CSS-Tricks](https://css-tricks.com/snippets/html/glyphs/)
* [Free outline Iconset](http://linea.io/)
