# construct.oocss

A Object Oriented Cascading Style Sheet framework for modern browsers.

## Getting Started

Construct.oocss supports multiple sites using the same code-base. In the _imports.scss_ file, you will notice the first two _@imports_ statements import:


 __1. A Build File__

Build files contain variables that determine what components to include.

__2, A Theme File__

Theme files contain variables that determine the site's visual appearence.

* * *

### Changing the Build

In the _imports.scss_ file, change the following line to your desired Build file.

    @imports "builds/_default.scss";    

* * *

### Changing the Theme

In the _imports.scss_ file, change the following line to your desired Theme file.

    @imports "themes/_default.scss";    
