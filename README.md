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

## concepts:
- box-sizing
- initial value
- inheritance
- browser defaults
- `%`, `rem`, `em` (for font), `em` (for length), `vh` and `vw`

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
    