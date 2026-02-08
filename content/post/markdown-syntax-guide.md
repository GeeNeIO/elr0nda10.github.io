---
title: "Markdown Syntax Guide"
date: 2026-02-06T11:00:00+00:00
description: "A comprehensive guide to Markdown syntax with examples"
categories:
  - "Documentation"
tags:
  - "markdown"
  - "writing"
  - "reference"
thumbnail: ""
lead: "A quick reference guide for writing in Markdown - the simple markup language that powers this blog."
---

This post is a reference guide for Markdown syntax. Whether you're writing blog posts, documentation, or README files, Markdown makes it easy to format text without complex tools.

## Headings

Use `#` symbols for headings. More `#` means smaller heading.

```markdown
# H1 Heading
## H2 Heading
### H3 Heading
#### H4 Heading
##### H5 Heading
###### H6 Heading
```

## Emphasis

Make text **bold**, *italic*, or ***both***.

```markdown
*italic text* or _italic text_
**bold text** or __bold text__
***bold and italic*** or ___bold and italic___
```

## Lists

### Unordered Lists

- Item one
- Item two
  - Nested item
  - Another nested item
- Item three

```markdown
- Item one
- Item two
  - Nested item
  - Another nested item
- Item three
```

### Ordered Lists

1. First item
2. Second item
3. Third item
   1. Nested item
   2. Another nested item

```markdown
1. First item
2. Second item
3. Third item
   1. Nested item
   2. Another nested item
```

## Links

Create [inline links](https://geene.io) or reference-style links.

```markdown
[inline link](https://geene.io)
[link with title](https://geene.io "GeeNe Homepage")
```

## Images

![Alt text for image](https://via.placeholder.com/150 "Optional title")

```markdown
![Alt text](image-url.jpg "Optional title")
```

## Code

### Inline Code

Use `backticks` for inline code.

```markdown
Use `backticks` for inline code.
```

### Code Blocks

Use triple backticks with optional language specification:

```python
def hello_world():
    """A friendly greeting."""
    print("Hello, GeeNe!")

hello_world()
```

````markdown
```python
def hello_world():
    print("Hello, GeeNe!")
```
````

### Syntax Highlighting

Supported languages include: python, javascript, java, go, rust, bash, sql, json, html, css, and many more.

```javascript
const greeting = (name) => {
    return `Hello, ${name}!`;
};

console.log(greeting("World"));
```

## Blockquotes

> "The best way to predict the future is to invent it."
> — Alan Kay

> You can also nest blockquotes.
>> Like this.
>>> And this.

```markdown
> Single blockquote
>> Nested blockquote
```

## Horizontal Rules

Create horizontal lines with three or more hyphens, asterisks, or underscores:

---

```markdown
---
***
___
```

## Tables

| Syntax      | Description | Example       |
| ----------- | ----------- | ------------- |
| Header      | Title       | `<h1>`        |
| Paragraph   | Text        | `<p>`         |
| Link        | Hyperlink   | `<a>`         |

```markdown
| Syntax    | Description |
| --------- | ----------- |
| Header    | Title       |
| Paragraph | Text        |
```

### Table Alignment

| Left-aligned | Center-aligned | Right-aligned |
| :----------- | :------------: | ------------: |
| Left         | Center         | Right         |
| Text         | Text           | Text          |

```markdown
| Left-aligned | Center-aligned | Right-aligned |
| :----------- | :------------: | ------------: |
| Content      | Content        | Content       |
```

## Task Lists

- [x] Completed task
- [ ] Incomplete task
- [ ] Another task

```markdown
- [x] Completed task
- [ ] Incomplete task
```

## Footnotes

Here's a sentence with a footnote[^1].

[^1]: This is the footnote content.

```markdown
Here's text with a footnote[^1].

[^1]: This is the footnote.
```

## Strikethrough

~~This text is crossed out~~

```markdown
~~crossed out text~~
```

## Escaping Characters

Use backslash `\` to escape Markdown characters:

\*This text is not italic\*

```markdown
\*This text is not italic\*
```

## HTML in Markdown

You can use HTML directly in Markdown:

<div style="background: #f0f0f0; padding: 10px; border-radius: 5px;">
This is a custom styled div.
</div>

```html
<div style="background: #f0f0f0; padding: 10px;">
Custom HTML content
</div>
```

## Emoji Support

If enabled in Hugo config, you can use emoji shortcodes:

:smile: :heart: :rocket: :computer:

```markdown
:smile: :heart: :rocket:
```

## Mathematical Expressions

If MathJax is enabled, you can write mathematical formulas:

Inline math: $E = mc^2$

Block math:

$$
\frac{n!}{k!(n-k)!} = \binom{n}{k}
$$

```markdown
Inline: $E = mc^2$

Block:
$$
\frac{n!}{k!(n-k)!} = \binom{n}{k}
$$
```

## Best Practices

1. **Use headings hierarchically** - Don't skip levels (H1 → H3)
2. **Leave blank lines** around blocks (lists, code, quotes)
3. **Be consistent** with your style (dashes vs asterisks)
4. **Use meaningful link text** - Avoid "click here"
5. **Add alt text to images** for accessibility

## Useful Tips

- Preview your Markdown before publishing
- Most editors support Markdown shortcuts (Ctrl+B for bold, etc.)
- Keep lines reasonably short for readability in source
- Use linters like `markdownlint` for consistency

## Resources

- [Markdown Guide](https://www.markdownguide.org/)
- [GitHub Flavored Markdown](https://github.github.com/gfm/)
- [CommonMark Specification](https://commonmark.org/)

---

That's it! You now have a complete reference for Markdown syntax. Happy writing!

*This guide is continuously updated. Bookmark it for future reference.*
