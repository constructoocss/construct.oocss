# construct.oocss

Construct.oocss is a Sass-based object-oriented framework that allows multiple sites to use the same code-base. Pretty nifty. It accomplishes this by separating the components to include, from the typography, and from the source code. Are you confused yet? Great. Please read on so we can clear a few things up for you.

### Getting Started

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

     
