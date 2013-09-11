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
     
