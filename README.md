# gulp-px2rpx

WeChat Mini Program px to rpx converter

## Installation

```shell
$ npm install --save-dev gulp-px2rpx
```

## Usage

```js
const gulp = require('gulp');
const px2rpx = require('gulp-px2rpx');

gulp.task('default', function () {
  gulp.src('./css/*.css')
    .pipe(px2rpx({
        screenWidth: 750, // Default screen width: 750
        wxappScreenWidth: 750, // WeChat Mini Program screen width: 750
        remPrecision: 6 // Fractional precision, default 6
    }))
    .pipe(gulp.dest('./wxappCss'))
});
```
