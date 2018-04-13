# markdown-it-span

[![Build Status](https://img.shields.io/travis/pnewell/markdown-it-span/master.svg?style=flat)](https://travis-ci.org/pnewell/markdown-it-span)
[![NPM version](https://img.shields.io/npm/v/markdown-it-span.svg?style=flat)](https://www.npmjs.org/package/markdown-it-span)
[![Coverage Status](https://img.shields.io/coveralls/pnewell/markdown-it-span/master.svg?style=flat)](https://coveralls.io/r/pnewell/markdown-it-span?branch=master)

> `<span>` tag plugin for [markdown-it](https://github.com/markdown-it/markdown-it) markdown parser.

__v2.+ requires `markdown-it` v5.+, see changelog.__

`::spanned::` => `<span>spanned</span>`

Markup uses the same conditions as CommonMark [emphasis](http://spec.commonmark.org/0.15/#emphasis-and-strong-emphasis).


## Install

node.js, browser:

```bash
npm install markdown-it-span --save
bower install markdown-it-span --save
```

## Use

```js
var md = require('markdown-it')()
            .use(require('markdown-it-span'));

md.render('::spanned::') // => '<p><span>spanned</span></p>'
```

_Differences in browser._ If you load script directly into the page, without
package system, module will add itself globally as `window.markdownitSpan`.


## License

[MIT](https://github.com/pnewell/markdown-it-span/blob/master/LICENSE)
