

# Frontendler

[![Frontendler version](http://img.shields.io/badge/frontendler-v0.1.0-blue.svg?style=flat)](https://github.com/frontendler/frontendler)
[![Build Status](http://img.shields.io/travis/frontendler/frontendler.svg?style=flat)](https://travis-ci.org/frontendler/frontendler)

The responsive frontend kit.

Simple, efficient.

http://frontendler.com.br/

## Dependencies

Frontendler need Nodejs and Gulp to run.

NODE JS - [How to install](http://nodejs.org/)

GULP ```$ npm install gulp -g```

## Install

Install project node dependencies ```$ npm install```

##Run frontendler

watch
```
$ gulp watch
```

build
```
$ gulp build
```


## SASS

### GRID

grid-gutter

```scss
$grid-gutter: 40px;
```

grid-breakpoints

```scss
$grid-breakpoints:(
	phone: 100% max 480px,
	tablet: 100% min 481px max 768px,
	tablet-large: 100% min 769px max 1023px,
	desktop: 1024px min 1024px max 1199px,
	desktop-large: 1200px min 1200px
);
```
grid-row

```scss
@mixin grid-row()
```

grid-col

```scss
@mixin grid-col($col, $cols: 12, $gutter: $grid-gutter)
```

grid-col-breakpoint

```scss
@mixin grid-col-breakpoint($device, $col, $cols: 12, $gutter: false)
```
or
```scss
@mixin grid-col-breakpoint($device, $col, $cols: 12, $gutter: false){
	"optional custom css"
}
```

grid-breakpoint

```scss
@mixin grid-breakpoint($devices...){
	...
};
```

grid-breakpoint-hide

```scss
@mixin grid-breakpoint-hide ($devices...);
```

grid-breakpoint-show

```scss
@mixin grid-breakpoint-show ($devices...);
```

### THEME

theme-colors

```scss
$theme-colors:(
	ocean:   #00a7ca,
	blue:    #0075d3,
	purple:  #8244a7,
	pink:    #dd318a,
	green:   #71be48,
	yellow:  #f59d37,
	orange:  #f75925,
	red:     #dd202b,
	dark:    #1c2731,
	gray:    #606c78,
	silver:  #939fac
);
```

theme-color
```scss
@function theme-color($color-name,$amount:50%)
```
