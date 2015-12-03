karma-quixote
=============

[Quixote](https://github.com/jamesshore/quixote) for [Karma](http://karma-runner.github.io)

Installation
------------

Install the plugin from npm:

```sh
$ npm install karma-quixote --save-dev
```
Or from Github:

```sh
$ npm install 'git+https://github.com/woldie/karma-quixote.git' --save-dev
```

Instructions on how to install karma can be found [here](http://karma-runner.github.io/0.13/intro/installation.html)

## Configuration

In your Karma configuration:

* add `require('karma-quixote')` to the plugins list, and
* add `quixote` to the `frameworks` key

```js
// karma.conf.js
module.exports = function(config) {
  config.set({
    plugins: [ require('karma-quixote'), ... ],
  
    frameworks: ['quixote', ... ],
    
        .
        .
        .
  });
};
```

Usage
-----

This karma plugin simply loads and installs the global `quixote` namespace object.  It is your responsibility
to initialize a QFrame for Karma to add to its DOM and then make quixote assertions in your tests as described 
on the [Quixote](https://github.com/jamesshore/quixote) page

License
-------

The MIT License (MIT)
