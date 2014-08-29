futu-process-arrow
=====================

Simple [Polymer](https://github.com/Polymer/) component for drawing a process arrow
and showing the current stage.

![](docs/example.png)

There is a [demo page](http://futurice.github.io/futu-process-arrow/),
please have a look!


## Install

If you use Bower, you can simply

```sh
bower install --save futurice/futu-process-arrow
```

Otherwise, save the `futu-process-arrow.html` in your project manually.

## Usage

This is a Polymer component, so you need to have the Polymer Platform referenced in
your `<head>`. When that's done, just add an HTML import for `futu-process-arrow.html`
and use the element like so:

```html
<!-- in head -->
<link rel="import" href="bower_components/futu-process-arrow/futu-process-arrow.html">

<!-- in body -->
<futu-process-arrow
  selected="1">
  <span>Baby</span>
  <span>Child</span>
  <span>Teenager</span>
  <span>Working-class hero</span>
  <span>Retired</span>
</futu-process-arrow>
```
