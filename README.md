# construct.oocss


Construct.oocss is a lightweight, Sass-based object-oriented framework that uses [BEM](http://bem.info/)-style naming conventions.

## Configuration

### Overview

Inside _imports.scss_, you will notice the first two import statement point to:

__1. A Build File__

    @imports "builds/_default.scss";  

Build files contain variables that determine the components you want to use.

__2. A Theme File__

    @imports "themes/_default.scss";  
    
Theme files contain variables that determine the typography you want to use. 

### Creating a Build

__1. Make a copy from the original__

     copy builds/_default.scss builds/new-build.scss

__2. Edit the variables__
     
     $use-alert: true !default;
     
     $use-bar: true !default;

     $use-box: true !default;

     $use-btn: true !default;     
     .
     .
     .

__3. Change the following path in _imports.scss_ to the new file__

    @imports "builds/_default.scss";  
    
### Creating a Theme

__1. Make a copy from the original__

     copy themes/_default.scss builds/new-build.scss

__2. Edit the variables__
     
     $h1-size: 24px;
     
     $h2-size: 24px;

     $h3-size: 24px;     
     .
     .
     .

__3. Change the following path in _imports.scss_ to the new file__

    @imports "builds/_default.scss";  
     
## Swatching

### Overview

Inside the theme file, you will notice three sass lists.

__1. $swatch-classname__

    $swatch-classname
    {
        "white",
        "black",
        .
        .
        .
    }

Used to create a list of color skins based on the items in this list.

__2. $swatch-backcolor__

    $swatch-classname
    {
        #fff,
        #000,
        .
        .
        .
    }

Used to change the default background-color on each color skin.


__3. $swatch-forecolor__

    $swatch-classname
    {
        #000,
        #fff
        .
        .
        .
    }

Used to change the default foreground-color on each color skin.

### Considerations

There are somethings worth mentioning:

* Buttons will darken the color skin by 5% when the user presses it
* A --text modifier is added to each so you can use the background color as a foreground color


