---
title: "{{ .Name | humanize | title }}"
weight: 1
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---

# Get started with Visual Studio Code

VS Code is a fully integrated developement environment supporting Git and editing with simple preview.

## Install VS Code

1. [Download](https://git-scm.com/downloads) and install Git.
{{< hint info >}}
Default installation is fine. Don't worry if you don't unsterstand these options. VS Code will handle most Git interactions.
{{< /hint >}}
2. [Download](https://code.visualstudio.com/Download) and install VS Code.

## Clone your first repository

1. In your web browser, navigate to a repository.
2. Click `Code` and copy the HTTPS Git address.
3. From VS Code, select `View` > `Command Palette…`.
4. Enter and select `Git: Clone` > `Clone from GitHub`.
5. Enter the HTTPS Git address from above.
6. Login and authorize VS Code.
7. Select the folder where VS Code will store the working files for this repository.
8. Open the cloned repository.
