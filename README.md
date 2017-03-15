## Rock, Paper, Scissors

Browser based version of the game ‘Rock, Paper, Scissors’.

Don't know the game? http://en.wikipedia.org/wiki/Rock-paper-scissors

## What can it do?

- Ability to play against the computer
- Ability to simulate a game (Computer vs Computer)
- Ability to restart the game
- Computer generated plays are random.

## Tooling

The tooling we provide is the following:

- `webpack` to modularise your Javascript code
- `babel` to utilise ES6+ and Stage-3 features
- `node-sass` to modularise your styling via SASS
- `eslint` to make sure your code meets the standards
- `karma`, `mocha` and `chai` to help you write and run your unit tests in various browsers

## Install dependencies

To start developing, fork and clone the project first, then make sure you have Node.js *4.x* or higher.

You'll need `yarn` to install the dependencies we locked in via the `yarn.lock` checked in to this repo.

You can install `yarn` if you haven't done so via `brew install yarn`.

Once you have `yarn` installed, just run

```
$ yarn install
```

from the project folder.

## Helpful commands

Following CLI commands available:

- `yarn run dev` running `webpack-dev-server` and serving the project on `localhost`
- `yarn run test -- --browsers Chrome,Safari` running unit tests via `karma` e.g. in Chrome and Safari
- `yarn run lint` running `eslint` against your source (and config) files
- `yarn run build` running `webpack` build
- `yarn run serve` serving the `build/` folder contents

Whilst developing, you'll most likely to run `yarn run dev` in a terminal window, `webpack` will take care of everything, bundling your project to an in-memory `build/` folder and serving it from there. Also, `yarn run test` in another terminal window to see your tests running / failing on every file change which comes very handy if you're doing TDD.

If you'd like to see the output as files, just run `yarn run build` and the result will be found under a real `build/` folder.