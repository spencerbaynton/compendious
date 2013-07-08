# Compendious

A comprehensive, but concise, fluid 6 column grid system.

Each column's class name is prefixed with `c`, for _column_, but really because CSS class names cannot begin with a number. The digit that follows indicates which column to place the element in, not the span. To create a span from one column to another simply use a class name containing the start column and the end column sperated by a dash (`-`).

## Example

```html
<div class="cf">
	<div class="c1">15%</div>
	<div class="c2">15%</div>
	<div class="c3">15%</div>
	<div class="c4">15%</div>
	<div class="c5">15%</div>
	<div class="c6">15%</div>
	<div class="c1-c2">32%</div>
	<div class="c3-c4">32%</div>
	<div class="c5-c6">32%</div>
	<div class="c1-c3">49%</div>
	<div class="c4-c6">49%</div>
	<div class="c1-c6">100%</div>
</div>
```

## Clearing and Offsets

By using this class naming scheme, both clearing and offsets can be handled _automagically_.

```html
<div class="cf">
	<div class="c2">15%</div>
	<div class="c5">15%</div>
	<div class="c3-c4">32%</div>
	<div class="c2">15%</div>
	<div class="c5">15%</div>
</div>
```

## Compatibility

The `[attr|="name"]`, `[attr$="name"]`, and adjacent sibling (`+`) selectors are not supported by Internet Explorer 6.

## Inspiration

* [A better Photoshop grid for responsive web design](//elliotjaystocks.com/blog/a-better-photoshop-grid-for-responsive-web-design) —Elliot Jay Stocks
* [Gridset](//gridsetapp.com) (offsets and clearing)
* [Negative Grid](//chrisplaneta.com/freebies/negativegrid-fluid-css-grid-by-chris-planeta) (negative margin)