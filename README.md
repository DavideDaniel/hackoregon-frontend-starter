## Hack OR Front-End Starter

This is a starter kit for Hack Oregon front-end development using React + Redux.
This repo should help get started and keep the different projects aligned.

#### Getting Started
1. Get [Node 6.5 +](https://nodejs.org) - I recommend using [Node Version Manager](https://github.com/creationix/nvm).
2. `git clone https://github.com/hackoregon/hackor-frontend-starter.git`.
3. `npm i` - install
4. `npm start` - start dev mode (watching tests + linter)

Visit [localhost:3000](http://localhost:3000) in your browser to see the site.
Save changes to files and the site will automatically update. No need to refresh!

#### Running Tests

There are two options:

1. `npm test` - run tests
2. `npm run coverage` - run tests w/ coverage

Running tests with coverage will take longer, but it's good to know what lines still need testing. CI tooling with use the `npm run coverage` command.

Much like `npm start`, `npm test` will watch files and automatically print out the new test output. Watch it in your terminal.

#### Working with the [component library](https://github.com/hackoregon/component-library) and the project site at the same time

The component library is required by each project site using an npm dependency. Npm offers a utility called [`npm link`](https://docs.npmjs.com/cli/link) for using a local copy of a dependency when developing.

Once you have cloned both the component library and this project site, do the following:

1. `cd` to your local component-library checkout
2. Run `npm link`
3. `cd` to your local project site checkout
4. Run `npm link react-component-library`

Now any code in the project site that relies on components from the component library will import modules directly from your local checkout of component-library. Likewise, any changes you make to your local checkout of component-library will impact the project site. The project site will also watch these component-library changes and hot reload localhost:3000 for you.

#### Next up
- [ ]  Docs
- [ ]  Ability to remove reference files

[![Stories in Ready](https://badge.waffle.io/hackoregon/hackoregon-frontend-starter.png?label=ready&title=Ready)](http://waffle.io/hackoregon/hackoregon-frontend-starter)
