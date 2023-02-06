# Part 3 - Add a LaTeX export operation

In the groups from part 2, exchange your designs once again,
such that each group member now has a new design again
(i.e. one they did not make themselves and did not use in part 2).

> **Task**: Try to extend the design you were given 
> to support a `toLatex` function that exports
> the Markdown file as a LaTeX document.

You should think about and answer (in some form) the following questions:
- How much of the original design did you have to change?
  - How big are the changes?
  - Did the original design foresee those changes?
- Which properties of the design made the change easier/harder?

## Operations

### `toLatex`

`toLatex` generates a LaTeX document from the Markdown, i.e. from
```md
# Title
Some text
```

it would generate something like:

```tex
\documentclass{scrartcl}
\begin{document}
  \section{Some text}
  Some text
\end{document}
```
