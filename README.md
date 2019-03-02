# previewSlider

[![GitHub Issues](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/alikinvv/previewSlider/issues)  [![HitCount](http://hits.dwyl.com/alikinvv/previewSlider.svg)](http://hits.dwyl.com/alikinvv/previewSlider)  [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)  [![Donations Badge](https://yourdonation.rocks/images/badge.svg)](https://www.paypal.me/alikinvv)

previewSlider is a responsive fullscreen image slider where the users are able to preview next/previous image when hovering over the navigation arrows.

Clicking on the navigation arrows will transition to the next/prev image after a certain delay, with a countdown progress bar that tells the users how long it will take to start the transition.

:star: Star us on GitHub — it helps!

## [Live Demo](https://alikinvv.github.io/previewSlider/demo)

![aligment buttons](/demo/gif.gif?raw=tru)

## Options
 - `container` (object) - slider initialization container 
 - `arrowLeft` (object) - left arrow
 - `arrowRight` (object) - right arrow
 - `content` (boolean) - `true` to use div as slides, `false` to use img as slides | Default: `false`
 - `scale` (number) - zoom size in preview gallery | Default: `0.4`
 - `scrollSpeed` (number) - scroll speed in preview gallery | Default: `4`

## Usage

Example of the html markup for image slider:

```html
<div class="preview-slider">
    <div class="slider-wrapper">
        <img class="slider-item" src="https://new.powerfulphotography.co.uk/wp-content/uploads/2019/03/port-14.jpg" alt=""></div>
        <img class="slider-item" src="img/img2.jpg" alt=""></div>
        <img class="slider-item" src="img/img3.jpg" alt=""></div>
    </div>

    <div class="arrow arrow-right"></div>
    <div class="arrow arrow-left"></div>
</div>
```

Initialization for images slider:

```js
new previewSlider({
    container: '.preview-slider',
    arrowLeft: '.preview-slider .arrow-left',
    arrowRight: '.preview-slider .arrow-right',
});
```

Example of the html markup for conent slider:

```html
<div class="preview-slider">
    <div class="slider-wrapper">
        <div class="slider-item" style="background-image: url(img/img1.jpg)"></div>
        <div class="slider-item" style="background-image: url(img/img2.jpg)"></div>
        <div class="slider-item" style="background-image: url(img/img3.jpg)"></div>
    </div>

    <div class="arrow arrow-right"></div>
    <div class="arrow arrow-left"></div>
</div>
```

Initialization for conent slider:

```js
new previewSlider({
    container: '.preview-slider',
    content: true,
    arrowLeft: '.preview-slider arrow-left',
    arrowRight: '.preview-slider .arrow-right',
});
```

## License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/alikinvv/previewSlider/blob/gh-pages/LICENSE) file for details


[![Analytics](https://ga-beacon.appspot.com/UA-31485994-5/previewSlider-repo)](https://github.com/alikinvv/previewSlider)
