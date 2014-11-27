# useful.range.js: Range input element

An alternative for the HTML5 range input element.

Try the <a href="http://www.woollymittens.nl/useful/default.php?url=useful-range">demo</a>.

## How to include the script

The stylesheet is best included in the header of the document.

```html
<link rel="stylesheet" href="./css/useful-range.css"/>
```

This include can be added to the header or placed inline before the script is invoked.

```html
<script src="./js/useful-range.js"></script>
```

To enable the use of HTML5 tags in Internet Explorer 8 and lower, include *html5.js*.

```html
<!--[if lte IE 9]>
	<script src="//html5shiv.googlecode.com/svn/trunk/html5.js"></script>
<![endif]-->
```

## How to start the script

```javascript
var ranges = new useful.Range().init({
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

This project uses grunt.js from http://gruntjs.com/

The following commands are available for development:
+ `npm install` - Installs the prerequisites.
+ `grunt import` - Re-imports libraries from supporting projects to `./src/libs/` if available under the same folder tree.
+ `grunt dev` - Builds the project for development purposes.
+ `grunt prod` - Builds the project for deployment purposes.
+ `grunt watch` - Continuously recompiles updated files during development sessions.
+ `grunt serve` - Serves the project on a temporary web server at http://localhost:8000/ .

## License

This work is licensed under a Creative Commons Attribution 3.0 Unported License. The latest version of this and other scripts by the same author can be found at http://www.woollymittens.nl/
