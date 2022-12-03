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
        click you "{{< relref "#you" >}}"

        github[(fab:fa-github GitHub\nAnthrocon/docs)]
        click github "{{< relref "#github" >}}"

        hugo{{Hugo}}
        click hugo "{{< relref "#hugo" >}}"

        githubPages[GitHub Pages]
        click githubPages "{{< relref "#github-pages" >}}"

        cloudflare[Cloudflare]
        click cloudflare "{{< relref "#cloudflare" >}}"

        visitor(visitor\ndocs.anthrocon.org)
        click visitor "{{< relref "#visitor" >}}"

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

Hugo is a static website generator. This means all files are processed and stored ready to deliver. This differs from most websites that generate pages on-the-fly with each visit.

### GitHub Pages

GitHub Pages is a lightweight website server that stores and serves the finished website files.

### Cloudflare

Cloudflare is a global network of last-mile servers. It caches files, and handles the bulk of visitor requests.

### Visitor

A furry.
