 <p align="center">
  <a href="#"><img src="app/images/icon-128.png"/></a>
</p>

# GitHub Linker

[![Build Status][travis-image]][travis-url] [![Dependency Status][daviddm-url]][daviddm-image]

The GitHub Linker is a Google Chrome Extension which links [NPM](https://npmjs.org/), [bower](http://bower.io/), [Composer](https://getcomposer.org/) & [Duo](http://duojs.org) dependencies to their GitHub repository page. It also tries to link the `require()` value in a `.js`, `.jsx`, `.coffee` or `.md` file, with the related repository.

Many other GitHub pages like **Pull Request or Issues** will be supported too.

# Preview

![d](screencast.gif)



# Installation

[![Chrome Web Store][install-image]][webstore-url]



# require() examples
```
// Packages
require('fs') => http://nodejs.org/api/fs.html
require('lodash') => https://github.com/lodash/lodash

// File system
require('./index.js') =>  https://github.com/user/repo/blob/master/index.js
require('./utils/math.js') =>  https://github.com/user/repo/blob/master/utils/math.js

// Duo
require('user/repo') => https://github.com/user/repo
require('user/repo@master') => https://github.com/user/tree/master
require('user/repo@master:/folder/file.js') => https://github.com/user/repo/blob/master/folder/file.js
```



# Support
Should you have any problems, please open up an [issue](https://github.com/github-linker/chrome-extension/issues).



# License

Copyright (c) 2014 Stefan Buck. Licensed under the MIT license.

[webstore-url]: https://chrome.google.com/webstore/detail/github-linker/jlmafbaeoofdegohdhinkhilhclaklkp
[travis-url]: https://travis-ci.org/github-linker/chrome-extension
[travis-image]: https://travis-ci.org/github-linker/chrome-extension.svg?branch=master
[daviddm-url]: https://david-dm.org/github-linker/chrome-extension.svg?theme=shields.io
[daviddm-image]: https://david-dm.org/github-linker/chrome-extension
[install-image]: install.png
