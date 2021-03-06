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

/* empty space */
&nbsp; 

/* action box */
.cta 

/* center method with positioning absolute */

.card__cta {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
        }

.container {
     padding: 15rem 0;
}

background-size: 100%; ==  background-size: cover;

/* solid color gradient */
.book {
    background-image: linear-gradient( 105deg, 
    rgba($color-white, .9) 0%,
     rgba($color-white, .9) 50%,
     transparent 50%), 
     url(../img/nat-10.jpg);
    background-size: 100%;
    border-radius: 3px;
    box-shadow: 0 1.5rem 4rem rgba($color-black, 0.2);

    // testing purpose
    height: 50rem;
}

/* on bottom always */
padding: 1.5rem 2rem

&:focus:invalid {
    
}

```



### CSS property to remember

**clip-path**: creates a clipping region that sets what part of an element should be shown.

* **outline**(shorthand): An outline is a line that is drawn around elements, outside the borders, to make the element "stand out".

* **outline-offset**: dds space between an outline and the edge or border of an element.

*  **perspective**: it must be set on the parent of the 3D-positioned child we want to give it some perspective

* **backface-visibility**: Hide and show the back face an element

* **background-blend-mode**: defines the blending mode of each background layer (color and/or image). eg *background-blend-mode: screen;*

* **box-decoration-break**: specifies how the background, padding, border, border-image, box-shadow, margin, and clip-path of an element is applied when the box for the element is fragmented.

* **figure** tag specifies self-contained content

* **figcaption** defines a caption for a `<figure>` element.

* **shape-outside** defines a shape around which adjacent inline content should wrap.

** In order to **add space to a float element** use **transform: translate()** don't use margin or anything like that.

**there is no way to have transform property on one element** - they are working on it.

**filter** defines visual effects (like blur and saturation) to an element eg *filter: blur(3px) brightness(80%)*

**video** tag specifies a standard way to embed a video in a web page

**source** tag is used to specify multiple media resources for media elements

**object-fit: cover;** is used to specify how an <img> or <video> should be resized to fit its container.

**solid color gradient css**

**::input-placeholder pseudo-element:**

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
<a href="" class="btn-text">Learn more &rarr;</a>

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
* [Unsplash - Free beautiful images](https://unsplash.com/)
* [clip-path maker](https://bennettfeely.com/clippy/)
* [Free video for homepage](http://coverr.co/)

## live!
[Check here my project!](https://xenodochial-ritchie-156b6b.netlify.com/)