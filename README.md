# Rowupper JS Beautifier Config

Sharable js-beautify config used by Rowupper.

## Install

```sh
npm install --save js-beautify-config-rowupper
```

## Usage

Within your [js-beautify config object](https://github.com/beautify-web/js-beautify#loading-settings-from-environment-or-jsbeautifyrc-javascript-only) You can extend this configuration. This will serve as a base for your config, then you can make overrides in your own config object.

```js
const gulp = require('gulp');
const prettify = require('gulp-jsbeautifier');

gulp.task('...', () =>
  gulp.src(...)
    .pipe(prettify(require('js-beautify-config-rowupper')))
    .pipe(gulp.dest(...))
);
```
