---
title: "Blogging with Hugo and Github"
summary: "A walkthrough on how to setup and host a simple static blog site with Hugo and Github page."
date: 2023-12-30T09:24:00-06:00
tags:
  - web development
  - tutorial
author: "a_nightails"

draft: true
---
## Prerequisite

 - [Git](https://git-scm.com/) - version control.
 - [Github](https://github.com/) - for hosting.
 - [Hugo](https://gohugo.io/) - version v0.121.1 by time of writing.
 - [PaperMod](https://github.com/adityatelange/hugo-PaperMod) - the theme that I'm using, replace with your own if require.

### Git installation
For GNU/Linux, all distros should be shipped with Git installed by default.  If not, install via the distro's package manager.

For Windows and Mac, follow the instruction on the Git website.

If your website requires images or large binary files, install [GitLFS](https://git-lfs.com/) as well to track without bloating the repository.

Since I'm using Fedora, the command are:
- `sudo dnf install git`
- `sudo dnf install git-lfs`

### Github Repository
Create an empty public repository.

For the name of the repository:
- If you already have a domain purchased, then name however you want. The domain can be linked to the repository later.
- If you intent to use the `github.io` domain, then name it with this scheme `username.github.io`. Visit [Github Pages](https://pages.github.com/) for more info.


