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

        subgraph Markdown
            you <-- Git --> github
        end

        github --> hugo
        hugo --> githubPages

        subgraph HTML
            githubPages -.-> cloudflare
            cloudflare --> visitor
        end
{{< /mermaid >}}
