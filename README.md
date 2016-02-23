# jQuery Progress Bar

A lightweight jQuery plugin to animate a progress bar. This plugin is responsive.

<img src="http://i.imgur.com/Osre53K.jpg" alt="">

### Demo page

<a href="http://codepen.io/toplefty/full/xZoGEQ/">http://codepen.io/toplefty/full/xZoGEQ/</a>

### Installation

Include script after the jQuery library:

```html
<script type="text/javascript" src="/path/to/jquery-goal-slider.js"></script>
```
Recommended : use the scss file and customize easily the settings.

Alternatively you can include the css
```html
<link rel="stylesheet" href="/path/to/jquery-goal-slider.css"></script>
```

### Usage

In order to use this plugin you have to follow the provided html template. Some elements are optional : `.jgs__motivational` and `.jgs__steps-container`. Replace the text content at your convenance in those two containers.
```html
<div class="jgs__container">
    <div class="jgs__motivational">
        Help us reach
        <br> our goals.
    </div>
    <div class="jgs__image-container">
        <div class="jgs__percentage-container">
            <span class="jgs__percentage-value"></span>
        </div>
        <div class="jgs__overlay-container">
            <img class="jgs__overlay-image" src="OVERLAY IMAGE HERE">
        </div>
        <img class="jgs__image-base" src="ORIGINAL IMAGE HERE"/>
    </div>
    <div class="jgs__steps-container">
        <div class="jgs__steps-highlighted"></div>
        <div class="jgs__step">
            <span class="jgs__sum-goal">250 000 €</span>
            <span class="jgs__goal">Our first goal</span>
        </div>
        <div class="jgs__step">
            <span class="jgs__sum-goal">500 000 €</span>
            <span class="jgs__goal">Our second goal</span>
        </div>
        <div class="jgs__step">
            <span class="jgs__sum-goal">750 000 €</span>
            <span class="jgs__goal">Our third goal</span>
        </div>
        <div class="jgs__step">
            <span class="jgs__sum-goal">1 000 000 €</span>
            <span class="jgs__goal">Our fourth goal</span>
        </div>
    </div>
</div>

```

To init the plugin please do as follows :

```js
$('.jgs__container').progressBar( { options } );
```

### Options

#### easing (string)

An optional parameter to specify the animation easing. Defaults to easeOutCubic.

```js
easing: 'swing'
```

#### duration (number)

An optional parameter specifying the length of the animation in milliseconds (ms). Defaults to 6000 (6 seconds).

```js
duration: 2000
```

#### delay (number)

An optional parameter specifying the delay of the animation in milliseconds (ms). Defaults to 3000 (3 seconds)

```js
delay: 300
```

#### percentage (number)

The final value that you want the bar to be animated to.

```js
percentage: 42
```

#### slantDegree (number)

An optional parameter specifying the value of the slant. Defaults to 15. A value of `0` will disable the slant.

```js
slantDegree: 10
```

#### onStart (function)

A function to be called when the animation beings.

```js
onStart: function(){
  alert('The animation started')
}
```

#### onComplete (function)

A function to be called when the animation is complete.

```js
onComplete: function(){
  alert('The animation is over')
}
```

## License

MIT License
(c) [Antonin Cezard](https://www.linkedin.com/in/antonin-cezard-04a7a4a3)
