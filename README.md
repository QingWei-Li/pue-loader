# pue-loader

[![Build Status](https://img.shields.io/travis/QingWei-Li/pue-loader.svg?style=flat-square)](https://travis-ci.org/QingWei-Li/pue-loader)
[![npm](https://img.shields.io/npm/v/pue-loader.svg?style=flat-square)](https://www.npmjs.com/package/pue-loader)
![vue](https://img.shields.io/badge/vue-2.x-4fc08d.svg?colorA=2c3e50&style=flat-square)
[![](https://img.shields.io/badge/%24-donate-green.svg?style=flat-square)](https://github.com/QingWei-Li/donate)

> A more pythonic javascript for Vue component file.


## Usage

```pug
template
  div
    span {{ count }}
    button(@click="count++") +
    button(@click="count--") -

script
  export default {
    name: 'compo'
    data: () ->
      count: 0
  }

style
  span
    color red
```

## Installation
```shell
npm i pue-loader css-loader -D
```

webpack config

```javascript
modules.export = {
  module: {
    rules: [
      {
        test: /\.vue$/,
        loader: 'pug-loader'
      }
    ]
  }
}
```

## License
WTFPL
