---
title: "Overview"
weight: 1
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---

# Overview

Website workflow from you, the editor, to delivery.

{{< mermaid >}}
    %%{
        init: {
            "theme": "neutral"
        }
    }%%

    flowchart LR
        you(you)
        github[(fab:fa-github GitHub\nAnthrocon/docs)]
        hugo{{Hugo}}
        githubPages[GitHub Pages]
        cloudflare[Cloudflare]
        visitor(visitor\ndocs.anthrocon.org)

        subgraph fab:fa-markdown Markdown
            you <-- Git --> github
        end

        github --> hugo
        hugo --> githubPages

        subgraph fab:fa-html5 HTML
            githubPages -.-> cloudflare
            cloudflare --> visitor
        end
{{< /mermaid >}}

## Workflow

From text to website.

### You

With tools like [VS Code]({{< relref "Get started with VS Code" >}}), you'll edit website content in a language called Markdown.

### GitHub

Files are synchronized with an online respository hosted by GitHub. The synchronization protocol is Git. Git transfers files while maintaining a history of every change.

### Hugo

Anytime changes are made, Hugo generates finished HTML website files from Markdown.

### GitHub Pages

GitHub Pages is a lightweight website server that stores and serves the finished HTML files.

### Cloudflare

Cloudflare is a global network of last-mile servers. It caches files, and handles the bulk of visitor requests.

### Visitor

A furry.
