---
layout: default
title: "Useful Git Commands"
lang: en
---

## Useful Git commands

I could give pages of commands but let's focus on a handful that you'll probably use on a daily basis.

```bash
$> git rm --cached
# Remove the file from your staging area (un-track) but keep the file in your 
# working tree (your local disk)
# Example use-case is if you accidentally added a binary file

$> git log --oneline [--graph]
   34dda2c Create main.yml
   4b06f8a Upgrade to Gradle 6.1.1

$> git log --stat
# Shows the file changes with addition/deletion count

$> git commit --amend [--no-edit]
# Amend your previous commit with your "Staged" changes
# Side-effects
# General rule: do not amend commits you've pushed and that you're not the author of
```
