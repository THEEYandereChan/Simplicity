<h1 align="center">Simplicity</h1>

<div align="center">
  :steam_locomotive::train::train::train::train::train:
</div>
<div align="center">
  <strong>Aesthetic Based</strong>
</div>
<div align="center">
  A <code>Simplistic</code> theme with infinite possibility
</div>

<br />

<div align="center">
  <!-- Stability -->
  <a href="https://nodejs.org/api/documentation.html#documentation_stability_index">
    <img src="https://img.shields.io/badge/stability-experimental-orange.svg?style=flat-square"
      alt="API stability" />
  </a>
  <!-- NPM version -->
  <a href="https://npmjs.org/package/choo">
    <img src="https://img.shields.io/npm/v/choo.svg?style=flat-square"
      alt="NPM version" />
  </a>
  <!-- Build Status -->
  <a href="https://travis-ci.org/yoshuawuyts/choo">
    <img src="https://img.shields.io/travis/yoshuawuyts/choo/master.svg?style=flat-square"
      alt="Build Status" />
  </a>
  <!-- Test Coverage -->
  <a href="https://codecov.io/github/yoshuawuyts/choo">
    <img src="https://img.shields.io/codecov/c/github/yoshuawuyts/choo/master.svg?style=flat-square"
      alt="Test Coverage" />
  </a>
  
  </a>
  <!-- Standard -->
  <a href="https://standardjs.com">
    <img src="https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat-square"
      alt="Standard" />
  </a>
</div>

<div align="center">
  <h3>
    <a href="https://staplake.github.io/projects/">
      Website
    </a>
  </h3>
</div>

<div align="center">
  <sub>The Simple route. Made with ❤︎ by
  <a href="">THEE Yandere Chan</a> and
  <a href="https://github.com/THEEYandereChan/Simplicity/graphs/contributors">
    contributors
  </a>
</div>

## Table of Content
- [Features](#features)
- [Example](#example)
- [Installation](#installation)
- [See Also](#see-also)
- [Support](#support)

## Features
- __minimal size:__ weighing `4kb`, `choo` is a tiny little framework
- __event based:__ our performant event system makes writing apps easy
- __small api:__ with only 6 methods there's not much to learn
- __minimal tooling:__ built for the cutting edge `browserify` compiler
- __isomorphic:__ renders seamlessly in both Node and browsers
- __very cute:__ choo choo!

## Example
# Preview
![Preview](https://vgy.me/5UweEN.png)
Want to see more examples? Check out the [Choo handbook][handbook].

### Is Simplicity Discord ready?
Sure.

## API
This section provides documentation on how each function in `Simplcity` works. It's
intended to be a technical reference. If you're interested in learning choo for
the first time, consider reading through the [handbook][handbook] first
:sparkles:

### `app = choo([opts])`
Initialize a new `choo` instance. `opts` can also contain the following values:
- __opts.history:__ default: `true`. Listen for url changes through the
  history API.
- __opts.href:__ default: `true`. Handle all relative `<a
  href="<location>"></a>` clicks and call `emit('render')`

### `app.use(callback(state, emitter))`
Call a function and pass it a `state` and `emitter`. `emitter` is an instance
of [nanobus](https://github.com/yoshuawuyts/nanobus/). You can listen to
messages by calling `emitter.on()` and emit messages by calling
`emitter.emit()`.

See [#events](#events) for an overview of all events.

### `app.route(routeName, handler(state, emit))`
Register a route on the router. The handler function is passed `app.state`
and `app.emitter.emit` as arguments. Uses [nanorouter][nanorouter] under the
hood.

See [#routing](#routing) for an overview of how to use routing efficiently.

### `app.mount(selector)`
Start the application and mount it on the given `querySelector`. Uses
[nanomount][nanomount] under the hood. This will _replace_ the selector provided
with the tree returned from `app.start()`. If you want to add the app as a child
to an element, use `app.start()` to obtain the tree and manually append it.

### `tree = app.start()`
Start the application. Returns a tree of DOM nodes that can be mounted using
`document.body.appendChild()`.

### `app.toString(location, [state])`
Render the application to a string. Useful for rendering on the server.

### `choo/html`
Create DOM nodes from template string literals. Exposes
[bel](https://github.com/shama/bel). Can be optimized using
[yo-yoify][yo-yoify].

## Installation
```sh
$ npm install choo
```






## License
[MIT](https://tldrlegal.com/license/mit-license)

[bankai]: https://github.com/yoshuawuyts/bankai
[bel]: https://github.com/shama/bel
[browserify]: https://github.com/substack/node-browserify
[budo]: https://github.com/mattdesl/budo
[es2020]: https://github.com/yoshuawuyts/es2020
[handbook]: https://github.com/yoshuawuyts/choo-handbook
[hyperx]: https://github.com/substack/hyperx
[morphdom-bench]: https://github.com/patrick-steele-idem/morphdom#benchmarks
[nanomorph]: https://github.com/yoshuawuyts/nanomorph
[nanorouter]: https://github.com/yoshuawuyts/nanorouter
[nanomount]: https://github.com/yoshuawuyts/nanomount
[yo-yo]: https://github.com/maxogden/yo-yo
[yo-yoify]: https://github.com/shama/yo-yoify
[unassertify]: https://github.com/unassert-js/unassertify
[window-performance]: https://developer.mozilla.org/en-US/docs/Web/API/Performance
