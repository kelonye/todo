
  ![](http://f.cl.ly/items/3l0r2s1C0d1Y1d3N202J/todo.png)

  Todo list component example app:

## Installation

 Of course have `component(1)` installed:
 
    $ npm install -g component

 Install express for the server, and the component dependencies:

    $ npm install
    $ make

## Running the app

    $ node app

## Implementations

  This repository has several branches to display several techniques 
  that may be applied to structure your application. So far we have
  the following:
  
    - `master` use separate `./client` and `./server` directories

## Implementation

  In this implementation both server and client components are
  located within the `./lib` directory. Each component may be
  made up of only server-side scripts, client, or both. For example
  `./lib/item`'s "index.js" file is the server portion for nodejs,
  while "item.js" is the client-side model.

## Components used

  - [page.js](https://github.com/visionmedia/page.js) for routing
  - [model](https://github.com/component/model) for models
  - [collection](https://github.com/component/collection) for model collections
  - [keyname](https://github.com/component/keyname) for keycode name strings
  - [reactive](https://github.com/component/reactive) for reactive templates

## License

  MIT
