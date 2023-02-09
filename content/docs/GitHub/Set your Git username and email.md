---
title: "Set your Git username and email"
weight: 10
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---

# Set your Git username and email

The Git protocol stores username and email information with commits you make. This is separate from your GitHub credentials.

## Set the username associated with commits

The Git username is displayed beside each commit.

{{< hint info >}}
Although it's possible to set any username, using your GitHub username will make troubleshooting much easier.
{{< /hint >}}

{{< tabs "username" >}}
{{< tab "VS Code" >}}
1. Open the terminal with `Terminal` ❯ `New Terminal`.
2. Set your username by entering `git config --global user.name "MaxHeadroom"`, substituting your own username.
3. Confirm your username by entering `git config --global user.name`.
{{< /tab >}}
{{< tab "Git CLI" >}}
1. Open Git Bash from your applications.
2. Set your username by entering `git config --global user.name "MaxHeadroom"`, substituting your own username.
3. Confirm your username by entering `git config --global user.name`.
{{< /tab >}}
{{< /tabs >}}

## Set the email address used for commits

The Git email address is used to link commits to your GitHub account.

{{< hint info >}}
GitHub provides a private email address for commits if you wish to keep your personal email private.

1. Sign into GitHub.
2. From the user menu at the top right, select `Settings`.
3. Select `Emails`.
4. Scroll to `Keep my email addresses private`, then copy your private address. It looks something like: 123456789+MaxHeadroom@users.noreply.github.com.
{{< /hint >}}

{{< tabs "email" >}}
{{< tab "VS Code" >}}
1. Open the terminal with `Terminal` ❯ `New Terminal`.
2. Set your email by entering `git config --global user.email "123456789+MaxHeadroom@users.noreply.github.com"`, substituting your own email.
3. Confirm your email by entering `git config --global user.email`.
{{< /tab >}}
{{< tab "Git CLI" >}}
1. Open Git Bash from your applications.
2. Set your email by entering `git config --global user.email "123456789+MaxHeadroom@users.noreply.github.com"`, substituting your own email.
3. Confirm your email by entering `git config --global user.email`.
{{< /tab >}}
{{< /tabs >}}

# Next steps

- [Add a spell checker to VS Code]({{< relref "Add a spell checker to VS Code" >}})
- [Learn the basics of Markdown]({{< relref "Learn the basics of Markdown" >}})
