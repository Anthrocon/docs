---
title: "Learn the basics of Markdown"
weight: 10
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---

# Learn the basics of Markdown

<i class="fab fa-markdown"></i> Markdown is a common formatting syntax. Markdown files are human-readable plain text files with the extension `.md`.

## Paragraphs

Start with basic paragraphes. Paragraph blocks are separated by an empty line.

## Text styles

Most used text formatting.

| Input | Result |
| :- | :- |
| `# Heading 1`<br />`## Heading 2`<br />`### Heading 3` | <h1>Heading 1</h1><h2>Heading 2</h2><h3>Heading 3</h3> |
| `**Bold**` | **Bold** |
| `*Italic*` | *Italic* |
| `~~Strikethrough~~` | ~~Strikethrough~~ |

## Elements

Most used structural elements.

| Input | Result |
| :- | :- |
| <pre><code>> ## Blockquote<br />><br />> Lorem ipsum</pre></code> | <blockquote><h2>Blockquote</h2><p>Lorem ipsum</p></blockquote> |
| <pre><code>- First item<br />&nbsp;&nbsp;&nbsp;&nbsp;- Sub item<br />- Second item</pre></code> | <ul><li>First item<ul><li>Sub item</li></ul></li><li>Second item</li></ul> |
| <pre><code>1. First item<br />&nbsp;&nbsp;&nbsp;&nbsp;- Sub item<br />2. Second item</pre></code> | <ol><li>First item<ul><li>Sub item</li></ul></li><li>Second item</li></ol> |
| <pre><code>- [x] Task one<br />&nbsp;&nbsp;&nbsp;&nbsp;- [x] Sub task<br />- [ ] Task two</pre></code> | <ul><li><input checked disabled type="checkbox"> Task one<ul><li><input checked disabled type="checkbox"> Sub task</li></ul></li><li><input disabled type="checkbox"> Task two</li></ul> |

## Links

URLs can be absolute paths.

`[Another website](https://www.anthrocon.org/)`

Internal paths should use Hugo shortcode to test validity, plus simplicity of relative internal file names.

`[Internal link]({{</* relref "Learn the basics of Markdown" */>}})`

## Images

Hugo shortcode to use. Image location is relative page bundle.

`{{</* img src="image.jpg" alt="A descriptive alt text" */>}}`

Markdown common image.

`![A descriptive alt text](image.jpg)`

{{< hint warning >}}
Use the Hugo shortcode instead to render modern picture element. This will generate WebP source sets for best visitor experience.
{{< /hint >}}

## Horizontal rule

Draw a horizontal rule with three dashes after an empty line.

{{< columns >}}
```markdown
Horizontal rule

---
```

<---><div style="margin-top: 1.5em;">

Horizontal rule

---

</div>
{{< /columns >}}

## Code block

Code blocks are fixed-width, verbatic blocks of computer code. Begin and end code blocks with three grave characters on their own lines. Add an optional language descriptor to the opening line to enable code highlighting.

{{< columns >}}
````markdown
```html
<img>
```
````

<---><div style="margin-top: 1.5em;">

```html
<img>
```

</div>
{{< /columns >}}
