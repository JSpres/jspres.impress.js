jspres.impress.js
============

It's a fork of the awesome work of [Bartek Szopka](https://github.com/bartaz) - [impress.js](http://bartaz.github.io/impress.js/#/bored) but modified to be used in our editor [JSpres](http://jspres.com).

Here is a list of the most biggest changes from the original:
  - **hash support is disabled**

For our purposses we don't want to change the broswer's url on every step, so we decided to turn this off. It's still in the code (commented), so if you want to use this version of the code you can enable it easily.

  - **reinitSteps()**

We are extending the API with a custom function which is used to reinitialize the steps when a new slide is added, removed or changed dynamically from our editor.

  - **substeps**
The substeps are a part that every presentation should have and this is one of the main cons of the impress.js project.
Now with this patch you can add a ```substep``` class to every element inside a step in you don't have to warry for anything else. We will move on every substep in a slide. For now we do not support inline animations and transitions for the substeps so you can style them with CSS. All you have to know is the classes which specifies their state.
There are 3 classes - ```past```, ```entered``` and ```future``` and I think that their names are enough to understand them. 

** Warning **
This version is still under dev and we make changes now, so if you find any bugs or problems you can nottify us with opening an issue or simply contribute to the project to fix them.

  

# About JSpres

We should flll that info, but for now it's just a TODO

# About impress.js
It's a presentation framework based on the power of CSS3 transforms and transitions in modern browsers and inspired by the idea behind prezi.com.

If you want to learn more about impress.js go to the official repo [here](https://github.com/bartaz/impress.js).


LICENSE
---------

Copyright 2011-2012 Bartek Szopka

Released under the MIT and GPL (version 2 or later) Licenses.


