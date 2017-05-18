# Development methodology at Soixante circuits

In the following document we will describe the type of development process we are aiming at when we work together.

We will mainly develop our project with the vue framework (https://vuejs.org/). We use the v2 version and the template [soixantecircuits/nd](https://github.com/soixantecircuits/nd)

- We will always prefere to use robust library or vanilla JS instead of jQuery or Motools plugins. You can first seach on the following links to find you happiness: https://github.com/soixantecircuits/awesome-app-js

If you can not find anything, we encourage you to search on site such as:

- [http://npmjs.com/](http://npmjs.com/)
- [https://libraries.io/](https://libraries.io/)
- [https://www.javascripting.com/](https://www.javascripting.com/)
- [http://microjs.com/#](http://microjs.com/#)

You can download, test, create some demo on [codepen.io](http://microjs.com/#) and then add the library you selected to https://github.com/soixantecircuits/awesome-app-js

In general when developing a new application:

- We focus on KISS: Keep It Simple Stupid
- We try to stay DRY
- We avoid at all cost the use of bad habits, see #bad-habits
- We use babel, so you can play with ES6
- We will prefere vue-component in favor of custom integration of vanilla lib
- We will favor Chrome only compatibility (we use Electron)
- We will avoid at all cost the use of web worker (which are not compatible with Electron - see [#797](https://github.com/electron/electron/issues/))
- We will always avoid zoom / pinch, and limit the zoom to 1 - see, https://github.com/soixantecircuits/nd/issues/28
- We will keep with something very simple in term of layout: few markups, no tables, no frameworks (bootstrap, foundation)
- We will keep the compatibility to the edge version of Chrome / Webkit. Which means you can use : css-grid, flexbox and fancy stuff available in latest Electron.
- We use reset stylesheet, preference is to: https://github.com/mblode/marx
- We use a common SCSS stylesheet for the whole project
- We will use scoped SCSS component in .vue file for specific styling of component
- We will focus on component behaviour and make sure each component is well designed and coded

- We use yarn for package management
- We use webpack for bundling

The default template that can allow to start a new project is: 
https://github.com/soixantecircuits/nd

### Bad habits

#### The Grid 
The code we write must stay modular. For instance, imagine we have a design with a grid of 2 by 2, the code you will produce will allow to make a grid of n by n. The cost of modifying the code later is something we do not want to have to face.

#### The navigation
Let say we have a navigation. Instead of creating a fixed sized navigation you will code something that can take an undeterminate number of navigation.

#### The sublevel in a tree
Instead of using a fixed level, you will use the power of recursive function to create infinite sublevel element.

#### The waterfall of switchcase of if else statement
If you found your-self in a waterfall of if/else/elseif/switch/case/default and it takes more than 4 lines, move to something configurable.
You can most of the case use an array of object which design, named object, functions and properties and use a foreach loop to iterate inside the case you met.