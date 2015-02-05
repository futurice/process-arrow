process-arrow
=====================

Simple [Polymer](https://github.com/Polymer/) component for drawing a process arrow
and showing the current stage.

![](docs/example.png)

There is a [demo page](http://futurice.github.io/process-arrow/),
please have a look!


## Install

If you use Bower, you can simply

```sh
bower install --save futurice/process-arrow
```

Otherwise, save the `process-arrow.html` in your project manually.

## Usage

This is a Polymer component, so you need to have the `polymer.html` referenced in
your `<head>`. When that's done, just add an HTML import for `process-arrow.html`
and use the element like so:

```html
<!-- in head -->
<link rel="import" href="bower_components/process-arrow/process-arrow.html">

<!-- in body -->
<process-arrow
  selected="1">
  <span>Baby</span> <!-- can be any element with textContent -->
  <span>Child</span>
  <span>Teenager</span>
  <span>Working-class hero</span>
  <span>Retired</span>
</process-arrow>

<!-- OR with data-bindings -->
<process-arrow
  selected="1">
  <template repeat="{{ stage in stages }}">
    <span>{{ stage }}</span>
  </template>
</process-arrow>
```

## License
BSD (3-clause)
