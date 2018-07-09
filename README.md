# range.js: Range input element

An alternative for the HTML5 range input element.

Try the <a href="http://www.woollymittens.nl/default.php?url=useful-range">demo</a>.

## How to include the script

The stylesheet is best included in the header of the document.

```html
<link rel="stylesheet" href="./css/useful-range.css"/>
```

This include can be added to the header or placed inline before the script is invoked.

```html
<script src="./js/useful-range.js"></script>
```

## How to start the script

```javascript
var ranges = new Range({
	'elements' : document.querySelectorAll('.classname');
	'title' : '{value}% ({min}-{max})',
	'support' : navigator.userAgent.match(/webkit|opera|msie 10/gi)
});
```

**ranges : {array}** - An array of all the instances of the script.

**title : {string}** - The text format of the popup label of the input element.

**support : {boolean}** - A test to determine which browsers have native support for the range input element.

## How to build the script

This project uses node.js from http://nodejs.org/

This project uses gulp.js from http://gulpjs.com/

The following commands are available for development:
+ `npm install` - Installs the prerequisites.
+ `gulp import` - Re-imports libraries from supporting projects to `./src/libs/` if available under the same folder tree.
+ `gulp dev` - Builds the project for development purposes.
+ `gulp dist` - Builds the project for deployment purposes.
+ `gulp watch` - Continuously recompiles updated files during development sessions.
+ `gulp serve` - Serves the project on a temporary web server at http://localhost:8500/.
+ `gulp php` - Serves the project on a temporary php server at http://localhost:8500/.

## License

This work is licensed under a Creative Commons Attribution 3.0 Unported License. The latest version of this and other scripts by the same author can be found at http://www.woollymittens.nl/
