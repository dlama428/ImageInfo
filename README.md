ImageInfo.js
==============

A handy helper object to get image info.

Requires [jQuery](http://jquery.com)

Usage:
```js
$.when(ImageInfo("file.png")).then
(
	function(e)
	{
		console.debug("Image is " + e.height + "px by " + e.width + "px");
	},
	function(err)
	{
		throw("FATAL: Could not load image");
	}
);
```