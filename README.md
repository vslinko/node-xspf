# node.js XSPF async parser

## Installation

```
npm install xspf
```

## Usage

```js
var Xspf = require('xspf'),
    util = require('util'),
    fs = require('fs');

fs.createReadStream('playlist.xspf');

new Xspf(res).on('track', function (track) {
    console.log(util.format('%s - %s', track['creator'], track['title']));
});
```
