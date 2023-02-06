# TuTinyMark 1.0 specification

Unless noted otherwise below, all text is interpreted as body text.
Additionally, TuSmallMark supports the following syntactic constructs:

## Paragraphs
Paragraphs are separated by blank lines, like this:

### Examples
```md
This is the first paragraph.

This is the second paragraph.
```

## Headings
Lines starting with one or more `#` are headings.

### Examples
```md
# Title of my document
Some text
## This is the first section
With more text
```

## Emphasis
Text enclosed in `*` is emphasized, which can be implemented as printing it in *italics*.

### Example
```md
Software Engineering is *not* the same thing as programming.
```

## Quotes
Successive lines starting with `> ` are interpreted as a quote. Quotes can be nested,
and all other elements can occur within quotes.

### Examples
```md
> This is a quote.
```

```md
> This is a multiline quote.
> That is, it has more than one line.
```

```md
> We can even nest quotes:
> > This is a nested quote.
```