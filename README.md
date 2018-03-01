# Gulp Prettier

[Prettier](https://github.com/jlongster/prettier)を使用してJavaScriptをフォーマットする[Gulp](http://gulpjs.com/)プラグイン

## 使用方法(Usage)

パス等は、適宜変更してください。

```js
const gulp = require('gulp');
const prettier = require('gulp-prettier');

gulp.task('default', () => {
  gulp.src('*.js')
    .pipe(prettier({
      useFlowParser: true
    }))
    .pipe(gulp.dest('./dist'))
});
```

## デフォルト設定(Defaults)

詳しい設定については、[Prettier](https://github.com/prettier/prettier)を参照してください。

```js
{
  printWidth: 80,
  tabWidth: 2,
  useFlowParser: false,
  singleQuote: false,
  trailingComma: false,
  bracketSpacing: true
}
```

## ライセンス(License)

[MIT License](https://raw.githubusercontent.com/bhargavrpatel/gulp-prettier/master/LICENSE)
