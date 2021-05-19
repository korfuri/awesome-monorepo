# Awesome Monorepo [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome Monorepo tools, software and
architectures. Monorepos, short for mono-repositories, are
repositories that contain multiple projects, usually related to each
other.

Inspired by [vinta/awesome-python](https://github.com/vinta/awesome-python).

## Contents

* [Build systems & dependency management tools](#build-systems--dependency-management-tools)
* [Repository management tools](#repository-management-tools)
* [Good reads](#good-reads)
* [Version control systems & add-ons](#version-control-systems--add-ons)
  * [Git](#git)
  * [Mercurial](#mercurial)
* [Development process tools](#development-process-tools)
* [Notable public monorepos](#notable-public-monorepos)
* [Migration tools](#migration-tools)

## Build systems & dependency management tools

* [baur](https://github.com/simplesurance/baur) builds only changed applications in a monorepo branch and manages build artifacts
* [Bazel](https://bazel.build) is Google's monorepo-oriented build system. More on Bazel: [awesome-bazel](https://github.com/jin/awesome-bazel)
* [Bit](https://github.com/teambit/bit) is a tool for building and managing JavaScript projects with multiple components, and managing the dependency graph of components.
* [Bolt Pkg](https://github.com/boltpkg/bolt) is a super-powered JavaScript project management.
* [Buck](https://buckbuild.com/) is Facebook's monorepo-oriented build system.
* [drkns](https://github.com/frantzmiccoli/drkns) a simple and language agnostic monorepo build tool.
* [Garment](https://github.com/Farfetch/garment) is Farfetch's monorepo build system with centralized and customizable task management.
* [GitLab CI](https://gitlab.com/gitlab-org/gitlab-ce/issues/19232) 11.4 supports running steps based on path changes.
* [Lerna](https://lerna.js.org/) is a tool for managing JavaScript projects with multiple packages, built on Yarn.
* [MBT](https://github.com/mbtproject/mbt) is a build tool with differential build support.
* [Nix](https://github.com/NixOS/nix) is a package and distribution build tool with remote caching, predominately used by NixOS.
* [Nx](https://nx.dev/) is a build system for TypeScript monorepos and a set of monorepo management tools.
* [OAO](https://github.com/guigrpa/oao) is a Yarn-based, opinionated JavaScript monorepo management tool.
* [Pants](http://www.pantsbuild.org/) is a monorepo-oriented build system, used by Twitter, Foursquare and multiple other companies.
* [Please](https://please.build/index.html) a cross-language build system with an emphasis on high performance, extensibility and reproduceability.
* [pnpm](https://pnpm.js.org/en/) is a JavaScript dependency management tool that supports monorepos through a set of dedicated commands called `pnpm multi`.
* [Rush Stack](https://rushstack.io/) is a family of tools geared towards large scale TypeScript monorepos, and based around the [Rush](https://rushjs.io/) build orchestrator
* [Spago](https://github.com/spacchetti/spago) is a PureScript package manager and build tool powered by Dhall and package-sets.
* [Symplify/MonorepoBuilder](https://github.com/Symplify/MonorepoBuilder) is a PHP monorepo management tool.
* [Tainted](https://github.com/kynrai/tainted) is a tool to determine which Go packages need to be rebuilt in a monorepo.
* [Yarn](https://yarnpkg.com/blog/2017/08/02/introducing-workspaces/) is a JavaScript dependency management tool that supports monorepos through workspaces.
* [Layer-pack](https://github.com/layer-pack/layer-pack) is a Webpack plugin allowing monorepo structures via inheritable npm packages/code layers & es6 glob imports.

## Repository management tools

* [Builder](https://github.com/FormidableLabs/builder) is a tool that makes it possible to ship the same scripts across projects in a Node.js monorepo. For example, share build and testing scripts across projects.
* [FBShipIt](https://github.com/facebook/fbshipit) is a library written in Hack for copying commits from one repository to another.
* [adeira/shipit](https://github.com/adeira/shipit) is a simplified JavaScript port of FBShipIt.
* [Lank](https://github.com/FormidableLabs/lank) is a tool that links packages together in a Node.js monorepo using automatic configuration of `NODE_PATH` instead of symlinks. Lank also allows you to run the same commands across all (or subsets of all) packages.
* [monorepo-run](https://github.com/Akryum/monorepo-run) is a collection of helpers to run scripts in each package of a yarn monorepo with a separated pane per package.
* [oao](https://github.com/guigrpa/oao)
* [Syncpack](https://github.com/JamieMason/syncpack) allows managing multiple package.json files in Lerna Monorepos.
* [Ultra Runner](https://github.com/folke/ultra-runner) is a smart script runner and build tool for Lerna, Pnpm, Rush and Yarn. Scripts run concurrently, using the dependency topology. Builds keep track of file changes and are skipped when possible.
* [wsrun](https://github.com/whoeverest/wsrun) allows running a command in each package of a Yarn workspaces monorepo.

## Good reads

* [Why Google Stores Billions of Lines of Code in a Single Repository](https://research.google.com/pubs/pub45424.html)
* [Advantages and Disadvantages of a Monolithic Repository: A case study at Google](https://people.engr.ncsu.edu/ermurph3/papers/seip18.pdf)
* [Why you should use a single repository for all your company’s projects](https://www.drmaciver.com/2016/10/why-you-should-use-a-single-repository-for-all-your-companys-projects/)
* [Advantages of monorepos](https://danluu.com/monorepo/)
* [Monorepos make inner-source come to life](https://kevingoslar.medium.com/monorepos-make-inner-source-come-to-life-bd1592b0cadf)
* [What is a monorepo? (and Should You Use Them?)](https://semaphoreci.com/blog/what-is-monorepo).

## Version control systems & add-ons

### Git

#### Tools

* [Git shallow clones](https://git-scm.com/docs/git-clone) let you clone only part of your Git history.
	* [How to Use Git Shallow Clone to Improve Performance](https://www.perforce.com/blog/git-beyond-basics-using-shallow-clones)
	* [How to handle big repositories with Git](https://www.atlassian.com/blog/git/handle-big-repositories-git)
	* [Git clones vs Shallow Git clones](https://blogs.gnome.org/simos/2009/04/18/git-clones-vs-shallow-git-clones/)
* [Git filter-branch](https://git-scm.com/docs/git-filter-branch) let you rewrite a repository's history and prune branches.
	* [How to handle big repositories with Git](https://www.atlassian.com/blog/git/handle-big-repositories-git)
* [Git clone --single-branch](https://git-scm.com/docs/git-clone)
	* [How to handle big repositories with Git](https://www.atlassian.com/blog/git/handle-big-repositories-git)
* [Git sparse-checkout](https://git-scm.com/docs/git-read-tree/)
	* [Cloning specific folders from git](https://lakehanne.github.io/git-sparse-checkout)
	* [How to handle big repositories with Git](https://www.atlassian.com/blog/git/handle-big-repositories-git)
* [Git LFS](https://git-lfs.github.com/) improves the handling of large files in Git.
* [GVFS](https://github.com/Microsoft/GVFS) virtualizes the file system beneath your git repo so that git and all tools see what appears to be a normal repo, but GVFS only downloads objects as they are needed. Windows only.
* [SlothFS](https://gerrit.googlesource.com/gitfs/+/HEAD/docs/manual.md) is similar to GVFS, but read-only. It works on Linux and macOS.
* [git subtree](https://github.com/apenwarr/git-subtree) merges and splits subtrees from your project into subprojects and back. Part of Git since version 1.7.
    * [git subsplit](https://github.com/dflydev/git-subsplit) automates and simplifies the process of managing one-way read-only subtree splits.
* [splitsh-lite](https://github.com/splitsh/lite) is a very fast git subtree alternative to splits subtrees from your project into subprojects.
* [josh](https://github.com/esrlabs/josh) is a git server proxy enabling on-the-fly virtualization of repositories.
* [go-diff](https://github.com/dstreamcloud/go-diff) is a handy tool analyzes which packages needed to be rebuilt due to changes.
* [mgt](https://github.com/nikita-skobov/monorepo-git-tools) is a tool that enables easy bidirectional sync between multiple repositories via files that define how to remap a repository

#### Scaling info

* Atlassian's [Monorepos in Git](https://developer.atlassian.com/blog/2015/10/monorepos-in-git/) and [How to handle big repositories in Git](https://www.atlassian.com/blog/git/handle-big-repositories-git) cover scaling options for Git.

### Mercurial

#### Tools

* [Watchman](https://github.com/facebook/watchman), replaced by [fsmonitor](https://www.mercurial-scm.org/wiki/FsMonitorExtension) trigger partial, incremental builds when your files change

#### Scaling info

* [Scaling Mercurial at Facebook](https://code.facebook.com/posts/218678814984400/scaling-mercurial-at-facebook/)

## Development process tools

### Code reviews

* [Pull Review](https://github.com/imsky/pull-review/) Hubot plugin to automate pull reviews with lots of configuration options.
* [Rietveld](https://github.com/rietveld-codereview/rietveld) is a code review tool by Google used by Chromium.
* [API Extractor](https://api-extractor.com/) is used to detect and review API signatures for TypeScript libraries, and also for publishing a multi-package API reference.

### CI tools

* [Incremental CI in Jenkins with Bazel](https://www.kchodorow.com/blog/2015/10/15/one-weird-trick-for-fast-ci/), article by Kristina Chodorow (Bazel team).
* [bazel-travis](https://github.com/korfuri/bazel-travis) is a minimal setup to use Travis CI in a Bazel monorepo.
* [buildpipe](https://github.com/jwplayer/buildpipe) is a tool to dynamically generate Buildkite pipelines by looking at changes in projects.
* [Codefresh](https://codefresh.io/) is a CI/CD platform for Docker/Kubernetes that has native [Monorepo support](https://codefresh.io/continuous-integration/using-codefresh-with-mono-repos/)
* [CI/CD for Microservices Using Monorepos](http://blog.shippable.com/ci/cd-of-microservices-using-mono-repos), a post describing a Shippable.com build designed for triggering builds specific to the microservice that has actually been modified and ones depending on it.
* [Semaphore CI](https://semaphoreci.com) is a CI/CD platform with native [monorepo support](https://docs.semaphoreci.com/essentials/building-monorepo-projects/).

### Code ownership

* [GitHub's CODEOWNERS](https://help.github.com/articles/about-codeowners/) can restrict who can approve a pull request that affects a given part of a monorepo.
* [Chromium's OWNERS file](https://chromium.googlesource.com/chromium/src/+/master/docs/code_reviews.md#OWNERS-files) inspired GitHub's CODEOWNERS.
* [Write Guard](https://github.com/geritol/write-guard) uses GitHub actions to enforce file-level write access to a monorepo.
* [CODEOWNERS generator](https://github.com/gagoar/codeowners-generator) generates a CODEOWNERS file for your monorepo from files in subfolders.

## Notable public monorepos

* [Foursquare's opensource projects](https://github.com/foursquare/fsqio)
* [Stellar's Go monorepo](https://github.com/stellar/go)
* [Habitat's monorepo](https://github.com/habitat-sh/habitat)
* [startup-os monorepo: working examples for Google's Open Source tools (bazel, etc) in a monorepo](https://github.com/google/startup-os)
* [M3 monorepo - Distributed TSDB, Aggregator and Query Engine, Prometheus Sidecar, Metrics Platform](https://github.com/m3db/m3)
* [Entria's Full Stack Playground Monorepo](https://github.com/entria/entria-fullstack)
* [Berty's monorepo - React-native mobile App + Golang backend + Gomobile bridge + iOS & Android native drivers + Protobuf](https://github.com/berty/berty/)
* [NixOS's monorepo of packages and modules can be used to incrementally build and deploy Linux machines](https://github.com/NixOS/nixpkgs/)
* [Celo's monorepo (includes blockchain, misc tooling, libraries, ops stuff like terraform modules, docs, etc)](https://github.com/celo-org/celo-monorepo)

## Migration tools

* [Bazel's migration-tooling](https://github.com/bazelbuild/migration-tooling) repository.
* [Gazelle](https://github.com/bazelbuild/rules_go#generating-build-files) generates Bazel BUILD files automatically for Go packages.
* [tomono](https://github.com/unravelin/tomono) imports an existing set of Git repositories into a monorepo.
* [shopsys/monorepo-tools](https://github.com/shopsys/monorepo-tools) contains a set of tools for building and splitting a monolithic repository.
* [Fastlane monorepo migration tools](https://github.com/fastlane/monorepo) tools for migrating code and github issues. Specific for fastlane so requires some code changes to use

## Development Workflows

* [Trunk Based Development](https://trunkbaseddevelopment.com), a source-control branching model, where developers collaborate on code in a single branch called ‘trunk’, resist any pressure to create other long-lived development branches by employing documented techniques. They therefore avoid merge hell, do not break the build, and live happily ever after.
* [Branch By Abstraction](https://www.branchbyabstraction.com), is a set-piece technique to effect a ‘longer to complete’ change in the trunk.

## License


[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)]("http://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, Uriel Corfa has waived all copyright and related or neighboring rights to this work.
