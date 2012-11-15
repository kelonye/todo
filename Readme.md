
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

<<<<<<< HEAD
  In this implementation all private client-side components are located in `./client`,
  while server related REST end-points are in `./server`. The `./index.html`
  file bootstraps the client-side, and `app.js` is a small Express server
  to power the backend.

  Each client-side component in `./client` defines its own dependencies,
  both "local" (in the `./client` dir), and remote from public components
  that devs have created. On `make` these are installed and the builder
  outputs `./build`. The tiny 1-line middleware in `./server/build` executes
  `make` on-demand each time `index.html` is requested, so you don't even
  have to know about the build

  This is just _one_ example of how you could structure an application. You could
  for example take a more traditional approach with `./models`, `./controllers`,
  and `./views` etc. The entire app could be a single component, with all dependencies
  specified in the root ./component.json, however I recommend splitting your app
  into multiple as shown here, regardless of directory structure.
=======
  In this implementation both server and client components are
  located within the `./lib` directory. Each component may be
  made up of only server-side scripts, client, or both. For example
  `./lib/item`'s "index.js" file is the server portion for nodejs,
  while "item.js" is the client-side model.
>>>>>>> add/alternative-structure

## Components used

  - [page.js](https://github.com/visionmedia/page.js) for routing
  - [model](https://github.com/component/model) for models
  - [collection](https://github.com/component/collection) for model collections
  - [keyname](https://github.com/component/keyname) for keycode name strings
  - [reactive](https://github.com/component/reactive) for reactive templates

## License

  MIT
