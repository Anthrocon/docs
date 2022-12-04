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

<i class="fab fa-markdown"></i> Markdown is a common formatting syntax. Markdown files are human-readable text files with the extension `.md`.

## Syntax

### Text styles

Most used text formatting.

| Syntax | Output |
| :--- | :--- |
| `# Heading 1`<br>`## Heading 2`<br>`### Heading 3` | <h1>Heading 1</h1><h2>Heading 2</h2><h3>Heading 3</h3> |
| `**Bold**` | **Bold** |
| `*Italic*` | *Italic* |
| `~~Strikethrough~~` | ~~Strikethrough~~ |

### Lists

Formatted lists are written as you'd like them to appear.

{{< columns >}}
Syntax

```markdown
- First item
- Second item
- Third item
```

<--->

Output

- First item
- Second item
- Third item
{{< /columns >}}

Numbered lists follow a similar syntax.

{{< columns >}}
Syntax

```markdown
1. First
    - Subpoint
        - Sub-subpoint
2. Second
```

<-->

Output

1. First
    - Subpoint
        - Sub-subpoint
2. Second
{{< /columns >}}

### Images

Hugo shortcode to use. Image location is relative page bundle.

`{{</* img src="image.jpg" alt="A descriptive alt text" */>}}`

Markdown common image.

`![A descriptive alt text](image.jpg)`

{{< hint warning >}}
Use the Hugo shortcode instead to render modern picture element. This will generate WebP source sets for best visitor experience.
{{< /hint >}}

### Links

URLs can be absolute paths.

`[Another website](https://www.anthrocon.org/)`

Internal paths should use Hugo shortcodes to test validity, plus simplicity of relative internal file names.

`[Internal link]({{</* relref "Learn the basics of Markdown" */>}})`

