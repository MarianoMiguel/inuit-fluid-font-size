# inuit-fluid-font-size

Fluid font-size mixin for [inuitcss](http://https://github.com/inuitcss/inuitcss).

## Installation

npm:

```
npm install --save inuit-fluid-font-size
```

yarn:

```
yarn add inuit-fluid-font-size
```

bower:

```
bower install inuit-fluid-font-size
```

At last, import the plugin inside the *tools* layer of your main or *manifest*
file:

```scss
@import "node_modules/inuit-fluid-font-size/tools/tools.fluid-font-size";
```

## How it works

The idea is to make fluid typography as simple and intuitive as possible: just
provide your desired font-size in pixels, and the mixin will make the calculations
to ensure the element's font-size matches that exactly at the breakpoint you
provide (The default breakpoint is `1200px`, but you can override the
`$inuit-fluid-font-size-breakpoint`variable).

There are no min or max boundaries. What we have instead, is a numeric variable
called `$inuit-fluid-font-size-scale-rate` (default value is `0.85`), which
controls how agressive the function is at scaling your font-size both up and down 
based on viewport width.
