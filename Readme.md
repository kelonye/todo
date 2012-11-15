
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

## Implementation

  In this implementation the traditional MVC directory structure is used,
  separating components by domain instead of by resource, into `./lib/controllers`, `./lib/models`, `./lib/views`.

## Components used

  - [page.js](https://github.com/visionmedia/page.js) for routing
  - [model](https://github.com/component/model) for models
  - [collection](https://github.com/component/collection) for model collections
  - [keyname](https://github.com/component/keyname) for keycode name strings
  - [reactive](https://github.com/component/reactive) for reactive templates

## License

  MIT
