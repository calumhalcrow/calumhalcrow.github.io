---
layout: post
title: "Export a commit range to patch files"
date: 2014-09-03 12:40
categories: git
---

Today I found myself in a position where a Git repo I am contributing to was to going to have its history significantly altered. Sensitive information was to be completely removed from the repo, and when done the repo would basically be a single commit on the master branch, with all other branches deleted.

<!-- more -->

But there were several open pull requests against master that would not get merged before this work was carried out. I had to save the commits in these PRs offline until the repo had been adjusted, then reapply them and re-open the PRs.

Here’s one way that this can be done:

## Commit range to patch files:

Ensuring you have your topic branch checked out and that it has some commits on it,

``` bash
$ git checkout topic-branch
$ git log --oneline origin/master..
898ea0f Adds more padding to footer.
c455b4f Makes header text blue.
```

you can make a patch out of each commit with the [git format-patch](http://git-scm.com/docs/git-format-patch) command:

``` bash
$ git format-patch origin/master..
0001-Makes-header-text-blue.patch
0002-Adds-more-padding-to-footer.patch
```

For each commit, we now have a patch file that can be saved offline and reapplied later:

``` bash
$ ls -l *.patch
-rw-r--r--  1 calum  staff  680 Sep  3 08:55 0001-Makes-header-text-blue.patch
-rw-r--r--  1 calum  staff  684 Sep  3 08:55 0002-Adds-more-padding-to-footer.patch
```

To reapply, move the patches to a directory outside of the repo (I moved mine to my home dir), checkout master and use the [git am](http://git-scm.com/docs/git-am) command:

``` bash
$ mv *.patch ~
$ git checkout master
Switched to branch ‘master'
$ git am ~/*.patch
Applying: Makes header text blue.
Applying: Adds more padding to footer.
```

Now the commits have be reapplied onto master. From here you can create a new branch, push it and re-open your pull requests.
