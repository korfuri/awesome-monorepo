# Awesome Monorepo

A curated list of awesome Monorepo tools, software and
architectures. Inspired
by [https://github.com/vinta/awesome-python](awesome-python).

#### Contents

## Build systems & dependency management tools

* [Bazel](https://bazel.build)
* [Pants](http://www.pantsbuild.org/)
* [Buck](https://buckbuild.com/)
* [Lerna](https://lernajs.io/)

## Repository management tools

* [oao](https://github.com/guigrpa/oao)
* [FBShipIt](https://github.com/facebook/fbshipit)

## Version control systems & add-ons

### Git

#### Tools

* [Git shallow clones](https://git-scm.com/docs/git-clone) let you clone only part of your Git history
	* [1](https://www.perforce.com/blog/git-beyond-basics-using-shallow-clones)
	* [2](https://www.atlassian.com/blog/git/handle-big-repositories-git)
	* [3](https://blogs.gnome.org/simos/2009/04/18/git-clones-vs-shallow-git-clones/)
* [Git filter-branch](https://git-scm.com/docs/git-filter-branch) let you rewrite a repository's history and prune branches.
	* [1](https://www.atlassian.com/blog/git/handle-big-repositories-git)
* [Git clone --single-branch](https://git-scm.com/docs/git-clone)
	* [1](https://www.atlassian.com/blog/git/handle-big-repositories-git)
* [Git sparse-checkout](https://git-scm.com/docs/git-read-tree/)
	* [1](https://lakehanne.github.io/git-sparse-checkout)
	* [2](https://www.atlassian.com/blog/git/handle-big-repositories-git)
* [Git LFS](https://git-lfs.github.com/) improves the handling of large files in Git.
* [GVFS](https://github.com/Microsoft/GVFS) virtualizes the file system beneath your git repo so that git and all tools see what appears to be a normal repo, but GVFS only downloads objects as they are needed. Windows only.
* [SlothFS](https://gerrit.googlesource.com/gitfs/+/HEAD/docs/manual.md) is similar to GVFS, but read-only. It works on Linux and OSX.

#### Scaling info

* Atlassian's [Monorepos in Git](https://developer.atlassian.com/blog/2015/10/monorepos-in-git/) and [How to handle big repositories in Git](https://www.atlassian.com/blog/git/handle-big-repositories-git) cover scaling options for Git.

### Mercurial

#### Tools

* [hgwatchman](https://bitbucket.org/facebook/hgwatchman) and [Watchman](https://github.com/facebook/watchman), replaced by [fsmonitor](https://www.mercurial-scm.org/wiki/FsMonitorExtension) trigger partial, incremental builds when your files change
* Facebook's [hg-experimental](https://bitbucket.org/facebook/hg-experimental/) extensions include better support for large repositories in Hg.

#### Scaling info

* [Scaling Mercurial at Facebook](https://code.facebook.com/posts/218678814984400/scaling-mercurial-at-facebook/)

## Code reviews

* [Rietveld](https://github.com/rietveld-codereview/rietveld) is a code review tool by Google used by Chromium

## CI tools

* [Incremental CI in Jenkins with Bazel](https://www.kchodorow.com/blog/2015/10/15/one-weird-trick-for-fast-ci/) by Kristina Chodorow (Bazel team)

## Code ownership

* [Github's CODEOWNERS](https://help.github.com/articles/about-codeowners/) can restrict who can approve a pull request that affects a given part of a monorepo
* [Chromium's OWNERS file](https://chromium.googlesource.com/chromium/src/+/master/docs/code_reviews.md#OWNERS-files) inspired Github's CODEOWNERS

## Notable public monorepos

* [Foursquare's opensource projects](https://github.com/foursquare/fsqio)
* [Stellar's Go monorepo](https://github.com/stellar/go)
* [Habitat's monorepo](https://github.com/habitat-sh/habitat)

## Migration tools

* [Bazel's migration-tooling](https://github.com/bazelbuild/migration-tooling) repository.
* [Gazelle](https://github.com/bazelbuild/rules_go#generating-build-files) generates Bazel BUILD files automatically for Go packages
* [tomono](https://github.com/unravelin/tomono) imports an existing set of Git repositories into a monorepo
