# scrollSpyder

A replacement for the twitter [scrollSpy](http://twitter.github.com/bootstrap/javascript.html#scrollspy) js plugin

## Usage

```javascript
$("#nav").scrollSpyder();
```

Or you can specify the amount of padding you want on the top of your dom element you are scrolling to:

```javascript
$("#nav").scrollSpyder({
  offset: 10
});
```

Where `#nav` is the id or class of the `<ul>` element containg your naviation.

**The recommended structure of navigation is:**

```html
<ul id="nav">
  <li class="active"><a href="#section-1">Link 1</a></li>
  <li><a href="#section-2">Link 2</a></li>
  <li><a href="#section-3">Link 3</a></li>
</ul>
```

> Navbar links must have resolvable id targets. For example, a `<a href="#section-1">Link 1</a>` must correspond to something in the dom like `<div id="section-1"></div>`.

## Quirks

* All `<li>` elements should be in the exact same order as their corresponding divs.