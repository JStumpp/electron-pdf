electron-pdf
============

[![NPM version][npm-image]][npm-url]
[![build status][travis-image]][travis-url]
[![Downloads][downloads-image]][downloads-url]
[![js-standard-style][standard-image]][standard-url]


A command line tool to generate PDF from URL, HTML or Markdown files with [electron](http://electron.atom.io/).

I have a blog post explain why [PDF Generation On The Web](https://fraserxu.me/2015/08/20/pdf-generation-on-the-web/)

![electron-pdf](https://cloud.githubusercontent.com/assets/1183541/9372796/6dc1089e-4715-11e5-8850-10dd9542aff8.gif)


Install
-------

```
npm install electron-pdf -g
```

Usage
-----

### Build PDF

```

  A command line tool to generate PDF from URL, HTML or Markdown files

  Options
    --help                     Show this help
    --version                  Current version of package
    -i | --input               String - The path to the HTML file or url
    -o | --output              String - The path of the output PDF
    -c | --css                 String - The path to custom CSS
    -b | --printBackground     Boolean - Whether to print CSS backgrounds.
                                 false - true
    -s | --printSelectionOnly  Boolean - Whether to print selection only
                                 false - default
    -l | --landscape           Boolean - true for landscape, false for portrait.
                                 false - default
    -m | --marginType          Integer - Specify the type of margins to use
                                 0 - default
                                 1 - none
                                 2 - minimum

  Usage
    $ electron-pdf <input> <output>
    $ electron-pdf <input> <output> -l

  Examples
    $ electron-pdf http://fraserxu.me ~/Desktop/fraserxu.pdf
    $ electron-pdf ./index.html ~/Desktop/index.pdf
    $ electron-pdf ./README.md ~/Desktop/README.pdf -l
    $ electron-pdf ./README.md ~/Desktop/README.pdf -l -c my-awesome-css.css

```

Inspired by [electron-mocha](https://github.com/jprichardson/electron-mocha)

### License

MIT

[npm-image]: https://img.shields.io/npm/v/electron-pdf.svg?style=flat-square
[npm-url]: https://npmjs.org/package/electron-pdf
[travis-image]: https://img.shields.io/travis/fraserxu/electron-pdf/master.svg?style=flat-square
[travis-url]: https://travis-ci.org/fraserxu/electron-pdf
[downloads-image]: http://img.shields.io/npm/dm/electron-pdf.svg?style=flat-square
[downloads-url]: https://npmjs.org/package/electron-pdf
[standard-image]: https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat-square
[standard-url]: https://github.com/feross/standard
