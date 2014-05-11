---
title: EmonHub Website
tags: 
categories: 
published: True
layout: default
js: index
---

### EmonHub website

The emonHub website is hosted on GitHub Pages

The [website's GitHub repository]({{site.web-git}}/blob/master/README.md)


Using GitHub pages to host the documentation website is an attempt to ease the task of documentation. Content is written almost entirely in markdown and the documents are then parsed directly to html pages automatically.

This method means that developers and users can contribute directly to the website using normal github procedures and has the intention of optimizing support as changes and solutions can be documented and updated more frequently than running a separate website.

##### Zen mode is perfect for this job 

----------------------------------------------------------------------------------------------------------

-------------------------------------------------------------------------------------------------------------

The `README.md` files are not use to compile the website but are a place to keep notes throughout the site, maybe using a `gitignore` could keep all the `README.md` docs on a `gh-pages-dev branch` and when changes are merged to `gh-pages` the `README.md` docs are not readily exposed. Bear in mind `emonhub master` will be the default branch. (will `.gitignore` work on branches ?)





##### The core of this site is based on `_includes` 
which can be reused and nested
the syntax is as follows



all `_includes` are located in the `_includes` folder in the root of the `gh-pages` branch of repo.
`_includes` can be sub divided into sub folders within the `_includes` folder, but it should be noted that once referenced in a page, if the `_includes` is moved, even within the `_includes` folder the link is broken.
the syntax to access "sub-foldered" `_includes` is simply by usual folder/file addressing[emoncmsorg]


note - a "page build failure" email is sent if any `_includes` cannot be resolved, identifying the page so can be rectified if `_includes` must be moved. (the page will also remain as it was prior to link breaking so will be out of date but not broken)

