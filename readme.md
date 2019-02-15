# bootstrap4-font-size-helper

Simple mixin which extends boostrap to help you  solve the font size in bootstrap defined breakpoints

- version 1.0.0
- last update 15/02/2019

## how to install and use
- Download package directly from github or install via ```npm install @kcko/bootstrap4-font-size-helper``` or with yarn ```yarn add @kcko/bootstrap4-font-size-helper```
- import ```_core.scss``` to your project via command ```@import "core";```
- generate required font sizes with ```@include bootstrap-font-size-maker();```

## mixin option
 * @param decimal|int $fontSizeStart - size from
 * @param decimal|int $fontSizeEnd - size to
 * @param decimal|int $step - step between size from and size to
 * @param string $separator - class separator between whole number  and decimal number eg: "-", and your class will looks like this ```fs-1_4``` (```1.4rem```), can be ommited or unfilled (empty string)
 * @param string $fontUnit - type of unit (rem, px, em, or any ...), default rem like in BS


## example of use
- ```@include bootstrap-font-size-maker(0.1, 5, 0.1, '');```
- ```@include bootstrap-font-size-maker(1, 10, 0.5, '_');```
- ```@include bootstrap-font-size-maker(1, 10, 0.2, '--', 'px');```

## in html
```html
<div class="fs-2 fs-sm-3 fs-md-4 fs-lg-5 fs-xl-6" style="padding: 1rem; margin: 1rem;">
  <div style="color: red;" class="d-block d-sm-none">xs</div>
  <div style="color: blue;" class="d-none d-sm-block d-md-none">sm</div>
  <div style="color: green;" class="d-none d-md-block d-lg-none">md</div>
  <div style="color: purple;" class="d-none d-lg-block d-xl-none">lg</div>
  <div style="color: gold;" class="d-none d-xl-block">xl</div>
  <div>
    Font size testing
  </div>
</div>
```




## video example
[![Watch the video](http://files.rjwebdesign.cz/i2/20190215-145503.png)](http://files.rjwebdesign.cz/f/20190215-162324.mp4)
