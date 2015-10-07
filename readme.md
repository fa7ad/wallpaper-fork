# wallpaper [![Build Status](https://travis-ci.org/sindresorhus/wallpaper.svg?branch=master)](https://travis-ci.org/sindresorhus/wallpaper) [![Build status](https://ci.appveyor.com/api/projects/status/xhwaihmhhplh5d05/branch/master?svg=true)](https://ci.appveyor.com/project/sindresorhus/wallpaper/branch/master)

> Get or set the desktop wallpaper

Works on OS X, Linux, and Windows.


## Install

```
$ npm install --save wallpaper
```


## Usage

```js
const wallpaper = require('wallpaper');

wallpaper.set('unicorn.jpg', err => {
	console.log('done');
});

wallpaper.get((err, imagePath) => {
	console.log(imagePath);
	//=> '/Users/sindresorhus/unicorn.jpg'
});
```


## API

### .get(callback)

#### callback(error, imagePath)

Type: `function`

##### imagePath

Type: `string`

Path to the current desktop wallpaper image.

### .set(imagePath, [callback])

#### imagePath

Type: `string`

Path to the image to set as the desktop wallpaper.


## Related

- [wallpaper-cli](https://github.com/sindresorhus/wallpaper-cli) - CLI for this module


## License

MIT © [Sindre Sorhus](http://sindresorhus.com)
