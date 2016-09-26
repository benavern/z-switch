![banner](img/banner.png)

# Z-Switch
Simple & stylish replacement for checkboxes, made with css only.

# [Demo](http://blog.caradeuc.info/z-switch)


## How to

### The default one : 

The simplest way to use it is with this html structure :

```html
<label class="z-switch">
    // text can go there
    <input type="checkbox">
    <div class="z-switch--container">
        <div class="z-switch--slider"></div>
    </div>
    // text can go there
    Hello, World!
</label>
```

![screenshot1](img/screenshot1.jpg)

#### Default checked ? 

If you want the checkbox to be checked by default, add it the `checked` attribute.

![screenshot1bis](img/screenshot1bis.jpg)

### ON & OFF labels

It is possible to add some text on the switchs to illustrate theire states. (max 3 chars)

For exemple here we will add "ON" & "OFF" labels : 

```html
<label class="z-switch">
    // text can go there
    <input type="checkbox">
    <div class="z-switch--container">
        <div class="z-switch--slider" data-on="ON" data-off="OFF"></div>
    </div>
    // text can go there
</label>
```

![screenshot3](img/screenshot3.jpg)

### Different sizes

Z-Switchs will always fit the parent font size, but it'zs possible to ask for smaller or bigger ones

2 classes can be added to the z-switch element 

* `z-switch-sm` : smaller one (font-size * 2/3)
* `z-switch-lg` : larger one (font-size * 4/3)

![screenshot2](img/screenshot2.jpg)

### Different shapes

Z-Switchs are circled by default, you can add these classes to change the shape :

* `z-switch-square`

![screenshotSquare](img/screenshotSquare.jpg)

* `z-switch-tictac`

![screenshotTictac](img/screenshotTictac.jpg)



### Different colors


#### The classes way

Two alternative colors are available for the switches, you can use it by adding classes 

* `z-switch-color1`

![screenshot4](img/screenshot4.jpg)


* `z-switch-color2`

![screenshot4bis](img/screenshot4bis.jpg)

#### The sass way

You can override the sass variables to change the switches colors, default ones are : 

```sass
// default colors
$z-switch-off    : #FF6059
$z-switch-on     : #2ACB41
$z-switch-slider : #FEFEFE
$z-switch-text   : #FEFEFE

// color1 alternative
$z-switch-color1-off    : #CCCCCC
$z-switch-color1-on     : #03A9F4

// color2 alternative
$z-switch-color2-off    : #FAFAFA
$z-switch-color2-on     : #FAFAFA
```
For example, if you want to reproduce the `z-switch-color1` class, you'll have to override variables this way :

```sass
$z-switch-off    : #CCCCCC
$z-switch-on     : #03A9F4
```


