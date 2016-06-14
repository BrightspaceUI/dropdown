**Looking for SASS-based `vui-dropdown`?** It's [over here](https://github.com/Brightspace/valence-ui-dropdown/tree/sass).

# d2l-dropdown
[![Bower version][bower-image]][bower-url]
[![Build status][ci-image]][ci-url]

A [Polymer](https://www.polymer-project.org/1.0/)-based web component for dropdown/flyouts.

## Installation

`d2l-dropdown` can be installed from [Bower][bower-url]:
```shell
bower install d2l-dropdown
```

## Usage

Include the [webcomponents.js](http://webcomponents.org/polyfills/) "lite" polyfill (for browsers who don't natively support web components), then import `d2l-dropdown.html`:

### Dropdown

```html
<head>
	<script src="https://s.brightspace.com/lib/webcomponentsjs/0.7.21/webcomponents-lite.min.js"></script>
	<link rel="import" href="../d2l-dropdown/d2l-dropdown.html">
</head>
```

Include the `d2l-dropdown` element on your page, and provide a `target-id` where the dropdown should open:

```html
<body>
	...
	<button id="my-opener">Open it!</button>
	<d2l-dropdown target-id="my-opener" >
		your content
	</d2l-dropdown>
</body>
```

Use the `opened` attribute to control the state of the dropdown.

```html
<body>
	...
	<d2l-dropdown opened target-id="my-opener" >
		your content
	</d2l-dropdown>
</body>
```

Optionally add the `no-auto-close` attribute to have the dropdown remain open when focus is lost.

```html
<body>
	...
	<d2l-dropdown no-auto-close target-id="my-opener" >
		your content
	</d2l-dropdown>
</body>
```

Optionally hide the pointer by specifying the `no-pointer` attribute.

```html
<body>
	...
	<d2l-dropdown no-pointer target-id="my-opener" >
		your content
	</d2l-dropdown>
</body>
```

### Usage in Production

In production, it's recommended to use a build tool like [Vulcanize](https://github.com/Polymer/vulcanize) to combine all your web components into a single import file. [More from the Polymer Docs: Optimize for Production](https://www.polymer-project.org/1.0/tools/optimize-for-production.html)...

## Coding styles

See the [VUI Best Practices & Style Guide](https://github.com/Brightspace/valence-ui-docs/wiki/Best-Practices-&-Style-Guide) for information on VUI naming conventions, plus information about the [EditorConfig](http://editorconfig.org) rules used in this repo.

[bower-url]: http://bower.io/search/?q=d2l-dropdown
[bower-image]: https://img.shields.io/bower/v/d2l-dropdown.svg
[ci-url]: https://travis-ci.org/Brightspace/d2l-dropdown-ui
[ci-image]: https://travis-ci.org/Brightspace/d2l-dropdown-ui.svg?branch=master
