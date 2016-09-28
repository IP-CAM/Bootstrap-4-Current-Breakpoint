# Bootstrap 4 Current Breakpoint
Simple solution for display current breakpoint in Bootstrap 4

![Bootstrap-4-Current-Breakpoint](/demo.gif)

Put this HTML in your page
```html
<div class="bootSizes">
    <div class="displaySize only-xs">XS</div>
    <div class="displaySize only-sm">SM</div>
    <div class="displaySize only-md">MD</div>
    <div class="displaySize only-lg">LG</div>
    <div class="displaySize only-xl">XL</div>
</div>
```

```scss
.bootSizes {
  position: fixed;
  z-index: 10;
  bottom: 0px;
  background: white;

  .displaySize {
    padding: 1rem;
  }
}

.only-xs,
.only-sm,
.only-md,
.only-lg,
.only-xl {
  display: none;
}

@include media-breakpoint-only(xs) {
  .only-xs {
    display: block;
  }
}

@include media-breakpoint-only(sm) {
  .only-sm {
    display: block;
  }
}

@include media-breakpoint-only(md) {
  .only-md {
    display: block;
  }
}

@include media-breakpoint-only(lg) {
  .only-lg {
    display: block;
  }
}

@include media-breakpoint-only(xl) {
  .only-xl {
    display: block;
  }
}
```
