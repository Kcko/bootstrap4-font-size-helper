# bootstrap4-font-size-helper
## version 1.0.0

Simple mixin which extends boostrap to help you  solve the font size in bootstrap defined breakpoints

## how to install and use
- Download package directly from github or install via ```npm install bootstrap4-font-size-helper```
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