<p align="center">
<img src="http://fapfapjs.io/img/logo.png" alt="Fapfapjs Logo"/>
<br/>Handcrafted javascript framework for DIY enthusiasts
<br/>http://fapfapjs.io/
</p>

# Getting started

Gulp & Grunt are awesome, why keeping one aside when we can use both!
Let's start the installation, you just have one line to run:
```
apt-get install ruby ruby-gem python nodejs build-essentials && \
    npm install -g yo && \
    yo fapfap && \
    configure && \
    make && \
    npm install && \
    bower update && \
    gulp build && \
    grunt serve && \
    gulp watch less
```
# Simple Hello World

As you could expect from a modern framework, FapfapJS is really simple to bootstrap. Here is an example to really feel the underneath power of the FAP (Federative Awesome Platform).
```js
/*global fapfap */
'use strict';

import Html exposing (attributes)

angular1      = require('angular1');
const react   = require('react');
let angular2  = require('angular2');
var mootool   = require('mootool');
const modules = require('*'); // just in case

(function (fapfap) {
  var DOMelement = document.body.innerHTML; // prepare triple-way-data-binding
  var hello = 'Hello World!';

  var [router, tool, door] = fapfap.unpack(modules, ['router', 'tool', 'door']);
  // uses our blazingly fast css selector pattern matching engine
  var partUnzipper = angular.module({'unzip': router.run('%body%').unzip()});

  // Close our DOM Object Ordering Recorder to prevent
  // from being interrupted by external process
  door.close();

  fapfap.stringFactory = partUnzipper.grab(tool);
  DOMelement = fapfap.stringFactory.createFromString(hello); // It's that easy
})(fapfap);
```

# Contributing

FapfapJS is so universal that anyone can bring his own expertise! The best way to do it is to open a pull request & submit your contribution. To help us identify the goal of your proposition, please follow the following guideline rules:

Please start your commit with:
- :fist: this commit is about a huge & hardcore refactor
- :open_hands: you did this commit in pair programming
- :punch: it made some BC Breaks
- :v: this was a quick & dirty fix
- :fu: promising experimental commit
- :muscle: improves the overall performances
- :sweat_drops: this may generate side effects
- :door: this commit improves the privacy
- :chestnut::chestnut: documentation improvement

## Still not convinced?
<p align="center">
<i>(Psst, you can click, it's a video)</i><br />
<a href="https://www.youtube.com/watch?v=JowtRcblp-U"><img src="https://img.youtube.com/vi/JowtRcblp-U/0.jpg" /></a>
</p>

# License
Fapfapjs is licensed under the MIT 2.0
