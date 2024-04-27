# eslint-config-google-jsdocless

> ESLint [shareable config](http://eslint.org/docs/developer-guide/shareable-configs.html) for the [Google JavaScript style guide (ES2015+ version)](https://google.github.io/styleguide/jsguide.html)

This is a fork of the original [eslint-config-google](https://github.com/google/eslint-config-google) project by [@andrewgjohnson](https://github.com/andrewgjohnson) to bring the original project into compliance with ESLint v9 now that `require-jsdoc` and `valid-jsdoc` have been deprecated.


## Installation

```
$ npm install --save-dev eslint eslint-config-google-jsdocless
```


## Usage

Once the `eslint-config-google-jsdocless` package is installed, you can use it by specifying `google-jsdocless` in the [`extends`](http://eslint.org/docs/user-guide/configuring#extending-configuration-files) section of your [ESLint configuration](http://eslint.org/docs/user-guide/configuring).

```js
{
  "extends": "google-jsdocless",
  "rules": {
    // Additional, per-project rules...
  }
}
```

### Using the `google-jsdocless` config with `eslint:recommended`

There are several rules in the [`eslint:recommended` ruleset](http://eslint.org/docs/rules/) that Google style is not opinionated about that you might want to enforce in your project.

To use Google style in conjunction with ESLint's recommended rule set, extend them both, making sure to list `google-jsdocless` last:

```js
{
  "extends": ["eslint:recommended", "google-jsdocless"],
  "rules": {
    // Additional, per-project rules...
  }
}
```

To see how the `google-jsdocless` config compares with `eslint:recommended`, refer to the [source code of `index.js`](https://github.com/google/eslint-config-google-jsdocless/blob/master/index.js), which lists every ESLint rule along with whether (and how) it is enforced by the `google-jsdocless` config.


## License

Apache-2 © Google
