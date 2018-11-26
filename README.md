# SoojungFirstPlugin

[![npm](https://img.shields.io/npm/v/soojung-first-plugin.svg)](https://www.npmjs.com/package/soojung-first-plugin) [![vue2](https://img.shields.io/badge/vue-2.x-brightgreen.svg)](https://vuejs.org/)

> A Vue.js Plugin

## Installation

```bash
npm install --save soojung-first-plugin
```

## Usage

### Bundler (Webpack, Rollup)

```js
import Vue from 'vue'
import SoojungFirstPlugin from 'soojung-first-plugin'
// You need a specific loader for CSS files like https://github.com/webpack/css-loader
import 'soojung-first-plugin/dist/soojung-first-plugin.css'

Vue.use(SoojungFirstPlugin)
```

### Browser

```html
<!-- Include after Vue -->
<!-- Local files -->
<link rel="stylesheet" href="soojung-first-plugin/dist/soojung-first-plugin.css"></link>
<script src="soojung-first-plugin/dist/soojung-first-plugin.js"></script>

<!-- From CDN -->
<link rel="stylesheet" href="https://unpkg.com/soojung-first-plugin/dist/soojung-first-plugin.css"></link>
<script src="https://unpkg.com/soojung-first-plugin"></script>
```

## Development

### Launch visual tests

```bash
npm run dev
```

### Launch Karma with coverage

```bash
npm run dev:coverage
```

### Build

Bundle the js and css of to the `dist` folder:

```bash
npm run build
```


## Publishing

The `prepublish` hook will ensure dist files are created before publishing. This
way you don't need to commit them in your repository.

```bash
# Bump the version first
# It'll also commit it and create a tag
npm version
# Push the bumped package and tags
git push --follow-tags
# Ship it 🚀
npm publish
```

## License

[MIT](http://opensource.org/licenses/MIT)
