jspres.impress.js
============

It's a fork of the awesome work of [Bartek Szopka](https://github.com/bartaz) - [impress.js](http://bartaz.github.io/impress.js/#/bored) but modified to be used in our editor [JSpres](http://jspres.com).

Here is a list of the most biggest changes from the original:
  - **hash support is disabled**
For our purposses we don't want to change the broswer's url on every step, so we decided to turn this off. It's still in the code (commented), so if you want to use this version of the code you can enable it easily.

  - **reinitSteps()**
We are extending the API with a custom function which is used to reinitialize the steps when a new slide is added, removed or changed dynamically from our editor.

  

# About JSpres

We should flll that info, but for now it's just a TODO

# About impress.js

If you want to learn more about impress.js go to the official repo [here](https://github.com/bartaz/impress.js).


LICENSE
---------

Copyright 2011-2012 Bartek Szopka

Released under the MIT and GPL (version 2 or later) Licenses.


