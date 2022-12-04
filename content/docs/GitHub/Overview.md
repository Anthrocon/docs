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

Website flow from editor to visitor visualised.

{{< mermaid >}}
    %%{
        init: {
            "theme": "neutral"
        }
    }%%

    flowchart LR
        editor(editor)
        click editor "{{< relref "#editor" >}}"

        github[(fab:fa-github\nGitHub)]
        click github "{{< relref "#github" >}}"

        hugo{{Hugo}}
        click hugo "{{< relref "#hugo" >}}"

        githubPages[GitHub Pages]
        click githubPages "{{< relref "#github-pages" >}}"

        cloudflare[fab:fa-cloudflare\nCloudflare]
        click cloudflare "{{< relref "#cloudflare" >}}"

        visitor(visitor)
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

## Component breakdown

From the moment an editor submits content, a chain of systems process and ready the website for delivery to visitors.

### Editor

With tools like [VS Code]({{< relref "Get started with VS Code" >}}), editors contribute content in [Markdown]({{< relref "Learn the basics of Markdown" >}}) — an easy to learn, human-readable text format.

### GitHub

Editors synchronize files with an online repository hosted by GitHub.

{{< hint info >}}
Git is a file transfer and versioning protocol, and is how GitHub gets its namesake. Every change, or `commit`, is recorded in detail allowing for unlimited reference and reversion.
{{< /hint >}}

### Hugo

Hugo is a static website generator. Once GitHub receives new content, Hugo automatically processes a complete website by turning Markdown into finished HTML.

By processing upfront, Hugo packages files that are immediately deliverable and viewable to a browser. In contrast, most other websites process on-the-fly, regenrating content with each visit.

### GitHub Pages

GitHub Pages is a lightweight web server that delivers the finished website files.

{{< hint info >}}
Since the files are ready for delivery to web browsers, GitHub Pages only passes the complete package to an intermediate content delivery network. The details of this serverless model are omitted for brevity.
{{< /hint >}}

### Cloudflare

Cloudflare provides a global network of last-mile servers. As the junction between Anthrocon and visitors, Cloudflare is responsible for caching files geographically near, and maintaining secure connections with visitors.

### Visitor

A furry.
