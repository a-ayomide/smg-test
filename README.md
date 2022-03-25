# react-redux-base (softcom.ng)

Forked from [react-redux-base](https://github.com/kenshinman/react-redux-base)

Preview at <http://chidimo.github.io/react-redux-base>

## Live preview

A live preview of this template is available at <http://chidimo.github.io/react-redux-base>

## Using scripts

1. To run tests, use command `yarn test`. Coverage report is automatically generated and placed in the `coverage/` folder. To view the report, open `/coverage/lcov-report/index.html`. You can have `jest` watch your files by running `yarn test:watch`.
1. To lint `JavaScript` files, run `yarn lint`. Optionally you can run `yarn lint --fix` to apply automatic fixes.
1. To prettify files, run `yarn pretty`. By default, the command prettifies `.ts`, `.js`, `.css`, `.html`, `.json`, and `.md` files. You may extend this list by adding more file extensions to the `pretty` section of `scripts` in `package.json`.

## Guides

### Prettification

1.  Add `.prettierrc` file to root of project. See available [configurations](https://prettier.io/docs/en/configuration.html) on the site.
1.  Install `prettier` as a development dependency.

        yarn add prettier -D

1.  Install [prettier-vscode](https://github.com/prettier/prettier-vscode) from the `vs-code` extension store.
1.  Create `pretty` script command.

### Linting

1. Add `.eslintrc.js` file to the root of the project.
1. Create `lint` script command

### Testing

1.  Add and configure `enzyme` test library. [Guide](https://alligator.io/react/testing-react-redux-with-jest-enzyme/)

        yarn add -D enzyme enzyme-adapter-react-16 enzyme-to-json
        yarn add -D redux-mock-store
        yarn add -D babel-jest @babel/core @babel/preset-env @babel/preset-react
        yarn add -D sinon chai
        yarn add -D @babel/plugin-proposal-class-properties

1.  Mock out css styles in jest

## Application layout structure

The app is laid out with a flexbox in such a way that no empty space will remain at the bottom. The app will completely occuppy the height of the viewport.

```html
<section id="root">
  <header>
    <nav></nav>
  </header>

  <main class="container">
    <section></section>
  </main>
</section>
```

## To Do

1. Add `prop-types` validation library and enable in `eslint`.
