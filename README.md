# Learning tips

* The best way to perform a basic reset using the universal selector

* How to set project-wide font definitions.

* How to clip parts of elements using *clip-path* property

## resources

* [CSS clip-path maker](https://bennettfeely.com/clippy/)

## Install NPM and Sass

* node -v
* npm init (open json file for us) to create a packet of json file
* npm install node-sass --save-dev

example;
* npm install jquery
* npm unistall jquery --save

```javascript
"script": {
    "compile:sass": "node-sass sass/main.scss css/style.css -w"
}
```
* `npm run compile:sass`

* `npm install live-server -g○` 
    * live-server

[Check here my project!](https://xenodochial-ritchie-156b6b.netlify.com/)

tips:

```css
&:not(:last-child){
        
    }
}

    .col-1-of-2 {
        width: calc((100% - #{$gutter-vertical}) / 2);
        background-color: orange;
        float: left;

        &:not(:last-child) {
            margin-right: $gutter-horizonatl;
        }
    }

    .col-1-of-3 {
        width: calc((100% - 2 * #{$gutter-vertical}) / 3);
        background-color: lightgreen;
        float: left;

        &:not(:last-child) {
            margin-right: $gutter-horizonatl;
        }
    }



/* select all the classes which start with col- */
[class^='col-']{}

    
/* select any classes which contain with col- */

[class*='col-']{}

/* select any classes which ends with col- */

[class$='col-']{}

```