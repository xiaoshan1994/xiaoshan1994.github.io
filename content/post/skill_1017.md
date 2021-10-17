---
title: "How effectively delete and add a git submodule"
date: 2021-10-17T17:47:11+02:00
description:
categories:
- Skill
- Code
tags:
- git
keywords:
- tech
coverImage:
coverSize:
thumbnailImage: https://miro.medium.com/max/343/0*p34AyEZYRw9kUY6e.png
thumbnailImagePosition: left
metaAlignment: center
---

Git Submodules are the concept related to modularity. One git repository can be added to another as a submodule and maintained separately. Instead of being tightly coupled, it is loosely coupled and is easy to maintain.<!--more-->Suppose you are working with software A which depends on library A, instead of copy-pasting the library A over and over again when a new version of the library is released what we can do is use submodule to make this process DRY and elegant.
### Delete
```
git submodule deinit <path_to_submodule>
git rm <path_to_submodule>
git commit -m "Removed submodule "
rm -rf .git/modules/<path_to_submodule>
```
### Add
```
git submodule add https://github.com/xiaoshan1994/hugo-tranquilpeak-theme.git themes/hugo-tranquilpeak-theme
```
{{< alert warning >}} If you try to add the submodule using `git submodule add`, you’ll need to delete the theme from themes and **push**. Otherwise, it’ll think it’s still in the index. {{< /alert >}}



{{< alert info/success/warning/danger >}} content {{< /alert >}}

{{< hl-text red >}} content {{< /hl-text >}}

{{< wide-image src="//d1u9biwaxjngwg.cloudfront.net/tag-plugins-showcase/car-1.jpg" title="Mercedes SLS" >}}
