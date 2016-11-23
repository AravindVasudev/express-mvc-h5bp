# express-mvc-h5bp
[![Dependency Status](https://www.versioneye.com/user/projects/5830ba58182815004288bb59/badge.svg?style=flat-square)](https://www.versioneye.com/user/projects/5830ba58182815004288bb59)

Boilerplate for Express using Express and html5 boilerplate.

##Stack
  This Boilerplate uses :
  * Backend -
    * Framework   - Express
    * Database    - MongoDB
    * ODM         - Mongoose.js
    * Templating  - Handlebars
    * Task Runner - Gulp
  * Frontend -
    * CSS Preprocessor - SCSS
    * ES6 Preprocessor - Babel
    * Libraries -
      * JQuery (Google CDN)
      * Bootstrap (Bootstrap CDN)
      * Modernizr
      * Normalize.css

##Quick Start
  * Clone this repository
  * Run `npm install`
  * Add your Database URL in config/database.js
  * Replace `public/favicon.ico` (optional)
  * Change `UA-XXXXX-X` in `views/layout.hbs` to your site's ID (optional)
  * Run `npm start` to run the server in port 3000

##Guide
  * Files -
    * Place SCSS files in `resources/scss`
    * Place client-side js in `resources/scripts`
    * Place unmodified static HTML files in `resources/html`
  * Layout -
    * The `views/layout` takes a meta object with `title`, `description`, `keyword` and `file` as properties
    * `file` property is the name of the CSS and JS file to be included (Assumes that the name of the Template, CSS and JS Files are the same)

##Gulp Tasks

| Task      | Description                                                                                                        |
|:---------:|--------------------------------------------------------------------------------------------------------------------|
| `images`  | minifies all the images in `public/img`                                                                            |
| `js`      | transpiles all js files in `resources/js` from es6 to es5, uglifies and places it in `public/js`                   |
| `css`     | transpiles scss files in `resources/scss` to css, autoprefixes them, minifies them and places them in `public/css` |
| `html`    | minifies html files in `resources/html` and places them in `public/`                                               |
| `build`   | runs `html`, `js`, `css` and `images`                                                                              |
| `watch`   | watches `html`, `css` and `js` files                                                                               |
| `default` | runs build and watch                                                                                               |

##License
The code is available under the [MIT license](LICENSE).
