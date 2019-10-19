# eslint-config-partylich [![Build Status](https://travis-ci.org/PartyLich/eslint-config-partylich.svg?branch=master)](https://travis-ci.org/PartyLich/eslint-config-partylich)

> ESLint [shareable config](http://eslint.org/docs/developer-guide/shareable-configs.html) based on the [Google JavaScript style guide (ES2015+ version)](https://google.github.io/styleguide/jsguide.html) with modifications to taste


## Installation

```
$ npm install --save-dev eslint eslint-config-partylich
```


## Usage

Once the `eslint-config-partylich` package is installed, you can use it by specifying `partylich` in the [`extends`](http://eslint.org/docs/user-guide/configuring#extending-configuration-files) section of your [ESLint configuration](http://eslint.org/docs/user-guide/configuring).

```js
{
  "extends": "partylich",
  "rules": {
    // Additional, per-project rules...
  }
}
```

### Using the `partylich` config with `eslint:recommended`

There are several rules in the [`eslint:recommended` ruleset](http://eslint.org/docs/rules/) that Google style (and PartyLich) are not opinionated about that you might want to enforce in your project.

To use this style config in conjunction with ESLint's recommended rule set, extend them both, making sure to list `partylich` last:

```js
{
  "extends": ["eslint:recommended", "partylich"],
  "rules": {
    // Additional, per-project rules...
  }
}
```

To see how the `partylich` config compares with `eslint:recommended`, refer to the [source code of `index.js`](https://github.com/PartyLich/eslint-config-partylich/blob/master/index.js), which lists every ESLint rule along with whether (and how) it is enforced by the `partylich` config.


## License

MIT © PartyLich
