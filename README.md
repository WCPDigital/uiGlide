[uiGlide jQuery Plugin](http://uiglide.com/) - An easy way to guide your users
================================

**A cross-browser, mobile-responsive JavaScript and jQuery plugin** for user interface (UI) guides, interactive application help and workflow demonstrations.

The uiGlide plugin supports all major browsers **(Chrome, Firefox, Safari, IE)** and will even work as as far back as **IE7+ if you include [Respond.js](https://github.com/scottjehl/Respond) and [html5shiv](https://github.com/aFarkas/html5shiv)**.

1. Appearance is controlled through CSS and can easily be restyled.
2. Animations and presentation can be enhanced through numerous timed callbacks.
3. Leverages HTML5 data attributes, but can be completely unobtrusive with all configuration set through JavaScript.
4. Lightweight: 12KB of JavaScript (less than 7KBs gzipped).

## Getting Started

### Try it out

jQuery demonstration: [See here](http://uiglide.com/uiGlide/examples/jQuery/)

Standalone demonstration: [See here](http://uiglide.com/uiGlide/examples/Standalone/)

### Downloading the prebuilt files

Prebuilt files, themes and examples can be downloaded from http://uiglide.com

### Including it on your page

Include jQuery, the uiGlide plugin and CSS theme file on a page. Then apply a few simple "data-" attributes to the areas on your page that you want to highlight or explain. Once ready, initialise the guide by calling the `uiGlide` method, followed by the `open` method.

```html
<head>
	<link href="uiglide.default.css" rel="stylesheet">
</head>
<body>
	<div data-uigset="demo_set" data-uigstep="0" data-uigtitle="My title" 
		data-uigdesc="My description" data-uightml="<p>Custom inner HTML content</p>">
	...
	</div>
</body>
<script src="jquery.js"></script>
<script src="jquery.uiglide.js"></script>
<script>
var uig = $("body").uiGlide().open();
</script>
```
Alternatively, if you don't use jQuery or want to incorporate uiGlide into your choice of library, you can use the `Standalone` version (which is almost the same in every way).

```html
<script src="uiglide.js"></script>
<script>
var uig = new uiGlide().open();
</script>
```

For more information on how to setup a rules and customizations, [check the documentation](http://uiglide.com/documentation/).

## Reporting issues and contributing code

See the [Contributing Guidelines](CONTRIBUTING.md) for details.

## License
Copyright &copy; WCP Digital &amp; Patrick Purcell<br>
Licensed under the [MIT license](http://www.opensource.org/licenses/mit-license.php).
