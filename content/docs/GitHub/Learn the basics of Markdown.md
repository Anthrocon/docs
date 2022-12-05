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

## Paragraphs

Start with basic paragraphes. Paragraphs are separated by an empty line.

## Text styles

Most used text formatting.

| Input | Result |
| :--- | :--- |
| `# Heading 1`<br />`## Heading 2`<br />`### Heading 3` | <h1>Heading 1</h1><h2>Heading 2</h2><h3>Heading 3</h3> |
| `**Bold**` | **Bold** |
| `*Italic*` | *Italic* |
| `~~Strikethrough~~` | ~~Strikethrough~~ |

## Lists

Formatted lists are written as you'd like them to appear.

{{< columns >}}

```markdown
- First item
- Second item
- Third item
```

<---><div style="margin-top: 1.5em;">

- First item
- Second item
- Third item

</div>
{{< /columns >}}

Numbered lists follow a similar syntax.

{{< columns >}}

```markdown
1. First
    - Subpoint
        - Sub-subpoint
2. Second
```

<---><div style="margin-top: 1.5em;">

1. First
    - Subpoint
        - Sub-subpoint
2. Second

</div>
{{< /columns >}}

## Images

Hugo shortcode to use. Image location is relative page bundle.

`{{</* img src="image.jpg" alt="A descriptive alt text" */>}}`

Markdown common image.

`![A descriptive alt text](image.jpg)`

{{< hint warning >}}
Use the Hugo shortcode instead to render modern picture element. This will generate WebP source sets for best visitor experience.
{{< /hint >}}

## Links

URLs can be absolute paths.

`[Another website](https://www.anthrocon.org/)`

Internal paths should use Hugo shortcode to test validity, plus simplicity of relative internal file names.

`[Internal link]({{</* relref "Learn the basics of Markdown" */>}})`

## Blockquotes

Create blockquotes similar to email.

{{< columns >}}

```markdown
> ## Hello
>
> How are you?
```

<---><div style="margin-top: 1.5em;">

> ## Hello
>
> How are you?

</div>
{{< /columns >}}
