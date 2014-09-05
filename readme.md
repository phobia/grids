# Grid

The grid system deals with horizontal space. To achieve vertical spacing, add bottom margin to the column content.

## Feature highlights

* Highly configurable
* Can be used both as classes in the HTML ("utility classes") and as mixins in LESS
* Supports responsive grids
* Supports fluid grid widths while maintaining fixed gutter
* Grids can be nested
* Span mixins supports fractions, e.g. `.span-(1/2)`.


## Introduction

By the default configuration, the grid system offers these functions:

<table class="kss-table">
  <thead>
  <tr>
      <td colspan="2"></td>
      <th>Class usage</th>
      <th>Mixin usage</th>
  </tr>
  </thead>
  <tbody>
    <tr>
      <th>row</th>
      <td>Defines a grid wrapper, contains columns.</td>
      <td>`.row`</td>
      <td>`.grid-row()`</td>
    </tr>
    <tr>
      <th>span</th>
      <td>Defines a column, and its width.</td>
      <td>`.span-#`</td>
      <td>`.grid-span(#)`</td>
    </tr>
    <tr>
      <th>push</th>
      <td>Move a column to the right.</td>
      <td>`.push-#`</td>
      <td>`.grid-push(#)`</td>
    </tr>
    <tr>
      <th>pull</th>
      <td>Move a column to the left.</td>
      <td>`.pull-#`</td>
      <td>`.grid-pull(#)`</td>
    </tr>
  </tbody>
</table>

By default, the grid row expands to the full width of its container. To limit the width add a `max-width` to the outer wrapper.

As you may notice, there are two methods of using the grid system:

1. By using **mixins** in LESS
2. By using **classes** in HTML

To minimize the HTML clutter, the first way is preferred, but there may be times when the latter is more practical. 

Either way, your grids are going to exist of three parts:

1. Grid wrapper, "row".
2. Grid column(s), "span".
3. Column content


