## Install

Install `@intelrug/stylint-loader` package

```bash
yarn install @intelrug/stylint-loader
```


## Usage

[Documentation: Using loaders](http://webpack.github.io/docs/using-loaders.html)

```javascript
module.exports = {
  // ...
  module: {
    rules: [
      {
        enforce: 'pre',
        test: /\.styl$/,
        loader: '@intelrug/stylint-loader'
      }
    ]
  }
  // ...
}
```


### Options

You can pass [stylint options](https://github.com/rossPatton/stylint#options) directly by

- Adding a query string to the loader for this loader usable only

```js
module.exports = {
  // ...
  module: {
    rules: [
      {
        enforce: 'pre',
        test: /\.styl$/,
        loader: '@intelrug/stylint-loader?{brackets: "never"}'
      }
    ]
  }
  // ...
}
```

- Adding an `options` entry:

```js
module.exports = {
  // ...
  module: {
    rules: [
      {
        enforce: 'pre',
        test: /\.styl$/,
        loader: '@intelrug/stylint-loader',
        options: {
          config: 'path/.stylintrc'
        }
      }
    ]
  }
  // ...
}
```

## [License](LICENSE)
