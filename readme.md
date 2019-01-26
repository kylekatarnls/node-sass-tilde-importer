# node-sass-tilde-importer

> A node-sass custom importer which turns `~` into absolute paths to the nearest parent `node_modules` directory.

[![Latest Stable Version](https://img.shields.io/npm/v/@kylekatarnls/node-sass-tilde-importer.svg?style=flat-square)](https://www.npmjs.com/package/@kylekatarnls/node-sass-tilde-importer)
[![Build Status](https://img.shields.io/travis/kylekatarnls/node-sass-tilde-importer.svg?style=flat-square)](https://travis-ci.org/kylekatarnls/node-sass-tilde-importer)
[![StyleCI](https://styleci.io/repos/167003001/shield?style=flat-square)](https://styleci.io/repos/167003001)
[![codecov.io](https://img.shields.io/codecov/c/github/kylekatarnls/node-sass-tilde-importer.svg?style=flat-square)](https://codecov.io/github/kylekatarnls/node-sass-tilde-importer?branch=master)

## Install

```sh
npm install @kylekatarnls/node-sass-tilde-importer --save-dev
```

## Usage

```js
var sass = require('node-sass');
var tildeImporter = require('@kylekatarnls/node-sass-tilde-importer');

var result = sass.renderSync({
  data: scss_content,
  importer: tildeImporter
});
```

`node-sass` cli example:
```sh
node-sass style.scss --importer=node_modules/node-sass-tilde-importer
```

Please refer to the node-sass [readme](https://github.com/sass/node-sass#readme) for full instruction on how to use custom importers.
