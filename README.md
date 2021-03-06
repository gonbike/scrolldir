<figure align="center">
  <img alt="scrolldir banner" src="https://cloud.githubusercontent.com/assets/1074042/22093384/09f3c2a6-ddba-11e6-8706-7e63be185448.jpg" />
</figure>
<p align="center">Leverage Vertical Scroll Direction with CSS 😎</p>

<hr>

<p align="center">
  <a href="https://travis-ci.org/dollarshaveclub/scrolldir/">
    <img alt="Build Status" src="https://travis-ci.org/dollarshaveclub/scrolldir.svg?branch=master" />
  </a>
  <a href="https://cdnjs.com/libraries/scrolldir">
    <img alt="CDNJS" src="https://img.shields.io/cdnjs/v/scrolldir.svg" />
  </a>
  <a href="https://www.npmjs.com/package/scrolldir">
    <img alt="npm version" src="https://badge.fury.io/js/scrolldir.svg" />
  </a>
  <a href="https://github.com/dollarshaveclub/scrolldir"> 
    <img alt="Bower version" src="https://badge.fury.io/bo/scrolldir.svg" />
  </a>
  <a href="https://twitter.com/home?status=ScrollDir%2C%20a%20micro%20JS%20lib%20that%20describes%20vertical%20scroll%20direction.%20https%3A%2F%2Fgithub.com%2Fdollarshaveclub%2Fscrolldir%20by%20%40pfisher42%20co%20%40yowainwright%20%40DSCEngineering">
    <img alt="Share on Twitter" src="https://img.shields.io/twitter/url/http/shields.io.svg?style=social&maxAge=2592000" />
  </a>
</p>

<hr>

<h1 align="center">ScrollDir ⬆⬇</h1>

ScrollDir, short for Scroll Direction, is a 0 dependency, ~1kb micro Javascript plugin to easily leverage vertical scroll direction in CSS via a data attribute. 💪

### ScrollDir is perfect for:
-  showing or hiding sticky elements based on scroll direction 🐥
-  tracking events on scroll direction 🔬
-  only changing its direction attribute when scrolled a significant amount 🔥
-  **ignoring small scroll movements** that cause unwanted jitters 😎

<hr>

## In Action🎥

<p align="center">
  <a href="https://dollarshaveclub.github.io/scrolldir/">
    <img src="https://cloud.githubusercontent.com/assets/1074042/22451992/ebe879b0-e727-11e6-8799-511209695e26.gif" alt="Scrolldir gif"  width="100%" />
  </a>
</p>

<hr>

## Install 📦

npm
```sh
npm install scrolldir --save
```
bower
```sh
bower install scrolldir --save
```
yarn
```sh
yarn add scrolldir 
```

## Setup 📤

### Auto
Add **dist/scrolldir.auto.min.js** and your done. There is no more configuration to do! Scrolldir will **just** conveniently work. 

### Default
Add **dist/scrolldir.min.js**. You have access to the API options below and must invoke scrollDir. See the [Default Setup Usage](#default) and [Options](#options) below.

<h2 id="default">Default Setup Usage 🛠</h2>

```javascript
scrollDir();
```
By default, ScrollDir will set the `data-scrolldir` attribute on the `<html>` element to `up` or `down`:

```html
<html data-scrolldir="up">
```
or
```html
<html data-scrolldir="down">
```

Now it's easy to change styling for vertical scroll direction!

```css
[data-scrolldir="down"] .my-fixed-header { display: none; }
```

<h2 id="options">Options ⚗</h2>

To use an attribute besides `data-scrolldir`:
```javascript
scrollDir({attribute: 'new-attribute-name'});
```
or
```javascript

```

To add the Scrolldir attribute to a different element:
```javascript
scrollDir({el: 'your-new-selector'});
```

To turn Scrolldir off:
```javascript
scrollDir({off: true});
```

## Examples 🌴

- [scrolldir](http://codepen.io/yowainwright/pen/9d5a6c6dcf2c17e351dcccfe98158e8b) on codepen.

This is a modular version of [pwfisher](https://github.com/pwfisher)'s [scroll-intent](https://github.com/pwfisher/scroll-intent.js). If you'd like to easily use scrolldir with jQuery—use Scroll Intent. ~TY!
