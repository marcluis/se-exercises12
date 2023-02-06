# Part 1 - Design a markdown library

In this task you will come up with a design for a simple library for TuTinyMark,
a (new) Markdown dialect.
This library must
- support all Markdown features described in `./specification.md`
- support two operations, `outline` and `toHTML`, described below.

> **Task**: Come up with a design for the library and document it with
> pictures (e.g. UML) and text on a sheet of paper.

You should think about and answer (in some form) the following questions:
- Which types/classes/traits/enums/... will have to be implemented?
  - How will they be related?
- Which methods/functions/... will there be?
  - What will be their type?
- What are likely future extenstions?
- Does your design adhere to the design principles from the lecture?
- Which other considerations influenced your design?

> **Note**: You will not have to implement the library.

## Operations

### `outline`

`outline` should generate an outline from the given Markdown document.
The outline is a tree of only the headings in the document, e.g.
```md
# A
Some text
## B
More text
### C
Even more text
## D
And finally some more
```
would generate an outline like the following:
> - A
>   - B
>     - C
>   - D

### `toHTML`
`toHTML` should render the Markdown file to HTML, i.e. generate a HTML document from it,
e.g. the following document:
```md
# Title
Some text
```
would result in something like
```html
<html>
  <body>
    <h1>Tile</h1>
    <p>Some test</p>
  </body>
</html>
```
