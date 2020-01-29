github-languages-css
===========
[![npm](https://img.shields.io/npm/v/github-languages-css.svg)](https://www.npmjs.com/package/github-languages-css)
> Stylesheet for creating colored elements based on a github language class

You do this in your markup.
```html
<span class='project__tag project__language--javascript'>javascript</span>
```

This is what you import/include in your css
```css
.project__language--javascript {
  background-color: #F1E05A;
  // the color is generated based on if white or black is a higher contrast to the background color
  color: #000000;
}
```

### Easy Installation

Just run `yarn add github-languages-css` or `npm install -save github-languages-css`

If you're using webpack to compile, you can use `@import '~github-languages-css/index.scss'`

If you're using postcss you can use `postcss-import` then `@import 'github-languages-css/index.css'`

If you're using a custom gulp / grunt task make sure your `includePath` for `node-sass` includes `node_modules`. Feel free to submit a issue if you have trouble setting this up.
