## Overview

The grid layout is based on CSS Grid’s two-dimensional system of columns and rows. This layout styles the parent element and its children to achieve responsive column and row spans as well as gutters.

## Usage

| Class | Applied to | Outcome |
| -- | -- | -- |
| `.pf-l-grid` | `<div>` | Initializes the grid layout. |
| `.pf-l-grid__item` | `<div>` | Explicitly sets a child of the grid. This class isn't necessary, but it is included to keep inline with BEM convention, and to provide an entity that will later be used for applying modifiers. |
| `.pf-m-gutter` | `.pf-l-grid` | Adds space between children by using the globally defined gutter value. |
| `.pf-m-all-{1-12}-col{-on-[breakpoint]}` | `.pf-l-grid` | Defines grid item size on grid container. |
| `.pf-m-{1-12}-col{-on-[breakpoint]}` | `.pf-l-grid__item` | Defines grid item size.  Although not required, they are strongly suggested. If not used, grid item will default to 12 col. |
| `.pf-m-{2-x}-row{-on-[breakpoint]}` | `.pf-l-grid__item` | Defines grid item row span.  For row spans to function correctly, the value of of the current row plus the grid items to span must be equal to or less than 12. Example: .pf-m-8-col.pf-m-2-row + .pf-m-4-col + .pf-m-4-col. There is no limit to number of spanned rows. |
