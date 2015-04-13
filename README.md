jspres.impress.js
============

It's a fork of the awesome work of [Bartek Szopka](https://github.com/bartaz) - [impress.js](http://bartaz.github.io/impress.js/#/bored) but modified to be used in our editor [JSpres](http://jspres.com).

Here is a list of the most biggest changes from the original:
  - **hash support is disabled**

For our purposses we don't want to change the browser's url on every step, so we decided to turn this off. We've added a way to configure ipmress on its initialization, you just have to pass a config object and we will do it. Here is an example how to disable the hash support:

```
var configuration = {
  isHashEnabled: false
};

var api = impress('impress', configuration);
api.init();
```

  - **reinitSteps()**

We are extending the API with a custom function which is used to reinitialize the steps when a new slide is added, removed or changed dynamically from our editor.

  - **substeps**

The substeps are a part that every presentation should contains and this is one of the main cons of the impress.js project.
Now with this patch you can add a ```substep``` class to every element inside a step and you don't have to wory about anything else. We will move on every substep in a slide. For now we do not support inline animations and transitions for the substeps but you can style them with pure CSS. All you have to know is the classes which specifies their state.
There are 3 classes - ```past```, ```entered``` and ```future``` and I think that their names are enough to understand how to use them. 

**Warning**
This version is still under dev and we make changes now, so if you find any bugs or problems you can nottify us with opening an issue or simply contribute to the project to fix them.

  - **basic styles**

Yes, right now the official imprss.js doesn't have a basic styles, it's jut contains only the styles for the demo presentation. We've filtered them and now the ```impress.css``` contains the basic styles which you need to start a new presentation.

** Warning**
This file contains basic styles for the browser interpreter and yhe impress.js messages, not skins for a better presentations. If you are looking for this you can take a look [here](https://github.com/JSpres/jspres-skins) and use our skins.
  

# About JSpres

We should flll that info, but for now it's just a TODO

# About impress.js
It's a presentation framework based on the power of CSS3 transforms and transitions in modern browsers and inspired by the idea behind prezi.com.

If you want to learn more about impress.js go to the official repo [here](https://github.com/bartaz/impress.js).


LICENSE
---------

Copyright 2011-2012 Bartek Szopka

Released under the MIT and GPL (version 2 or later) Licenses.


