# kalastatic-cli

Command line interface for KalaStatic.

## Install

### Globally

    $ npm install kalastatic-cli -g

### Project Dependency

To install KalaStatic as a dependency in your project:

    $ npm install kalstatic-cli --save

## Usage

### Write

Construct your source files, using the template engine name in the file extension.

#### src/index.html.jade
``` jade
---
youAreUsingJade: true
pretty: true
---
doctype html
html(lang="en")
  head
    title= title
  body
    h1 Jade - node template engine
```

### Build

#### Globally

    $ kalastatic

#### Project

    $ node_modules/.bin/kalastatic

## API

``` javascript
var KalaStatic = require('kalastatic')
KalaStatic('path/to/site').then(function() {
  // Site built
})
```
