# This is a readme file for the Natoure learning project

## things:
    -   clip-path
    -   animation
    -   display
    -   position
    -   transform
    -   background
    -   peseudo elements
    -   keyframes
    -   font
    -   backface-visitbility
    -   gradient
    -   box-shadow
    -   text
    -   floats

## concepts:
- box-sizing
- initial value
- inheritance
- browser defaults
- `%`, `rem`, `em` (for font), `em` (for length depends on font), `vh` and `vw`

## How the browser loads CSS:
Load HTML --> Parse HTML --> Load CSS --> (Resolve conflicts && Process final CSS value) --> CSSOM --> Render Tree -->
Render visual formatting model --> Render website

## 'cascade' meaning in CSS?
- Process of combining and resolve conflicting due to this order:
    1. Author
    2. User --> like changing font-size of a page by the user
    3. Browser (user agent) --> like default style of a link in browser

## How to resolve conflicts: importance > specificity > source order
- importance:
    1. user `!important`
    2. author `!important`
    3. author declaration
    4. user declaration
    5. browser declaration
- specificity (when we have same importance):
    1. inline styles
    2. IDs
    3. classes, pseudo-classes, attribute
    4. elements, pseudo-elements
- source order (when we have same specificity):
    1. last declaration in the code overrides

## Visual formatting model?
- box model
- box types
  - inline
    - distributed in lines
    - only content's spaces
    - no line-breaks
    - no heights and widths
    - padding and margin only horizontal (left and right)
  - block-level
    - (block, flex, list-item, table)
    - 100% of parent's width
    - vertically
    - box-model applied
  - inline-block
    - only content's spaces
    - no line-breaks
    - box-model applied

## positioning
- normal flow
  - default positioning
  - position: relative
- floats
  - text and inline elements wrap to the floated elements
  - the container will not adjust its to the element
- absolute positioning
  - position: absolute

## stacking context


## think - build - architect mindset
- think
  - component-driven design
  - atomic design
- build
  - BEM
  - OOCSS
  - SMACSS
- architect
  - 7-1 pattern (7 different folders for partial Sass files and 1 main Sass file to import all files):
    - `base/` --> basic definitions
    - `components/` --> one file for each component
    - `layout/` --> layout of the project
    - `pages/` --> styles of specific pages of the project
    - `themes/` --> for different visual themes
    - `abstracts/` --> variables & ...
    - `vendors/` --> all third-party css codes

# Sass
- color functions (like `darken()`, `lighten()`)
- mixins with arguments
- functions
- extend
- nesting
- variables
- difference between extend and mixin
- packages
  - node-sass

# Responsive Design Principles
- Fluid layout
  - adapt with viewport width or height
  - use `%`, `vh` or `vw` instead of `px`
  - use `max-width` instead of `width`
- responsive units
  - use `rem` instead of `px`
  - easy to scale down a page
- flexible images
  - fix images
  - use `max-width` and `%`
- media queries
  - use breakpoints

# Layout types
  - float
  - flexbox
  - grid