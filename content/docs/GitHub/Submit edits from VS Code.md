---
title: "Submit edits from VS Code"
weight: 1
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---

# Submit edits from VS Code

*Required reposity role: Write, Maintain, Admin*

After making edits, you can commit and sync changes to the repository.

## Commit changes

Git journals all changes. Before syncing files, you must record your changes as a `commit`.

1. From the menu, select `View` ❯ `Source Control`.
2. In `Message`, enter a short description of your changes.
{{< hint info >}}
A good message is short and describes why you made a change. "Fixes #123 Counting starts at 0 units" is an example of a good message. "Fixed variable" is a poor message because it doesn't describe what was done or why.
{{< /hint >}}
3. Click `Commit`.
4. When prompted to stage all changes, select `Yes`.

## Sync changes

You can make multiple commits, each with its own descriptive message. However, commits remain only on your computer until you sync changes to the repository.

1. From the menu, select `View` ❯ `Source Control`.
2. Under the respository you'd like to sync, click `Sync Changes`.
3. When prompted to pull and push commits, select `OK`.
