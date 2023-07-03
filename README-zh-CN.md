# Awesome Monorepo [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

一个精心策划的关于 Monorepo 工具、软件和架构的列表。
架构。Monorepos 是单库的简称，是指
储存库，包含多个项目，通常相互关联。
彼此相关。

灵感来自于 [vinta/awesome-python](https://github.com/vinta/awesome-python).

[English](./README.md) | 简体中文

## 内容

* [构建系统和依赖性管理工具](#构建系统和依赖性管理工具)
* [仓库管理工具](#仓库管理工具)
* [一些好的参考文献](#一些好的参考文献)
* [版本控制系统和附加组件](#版本控制系统和附加组件)
  * [Git](#git)
  * [Mercurial](#mercurial)
* [开发流程工具](#开发流程工具)
* [著名的公开 monorepos](#著名的公开-monorepos)
* [迁移工具](#迁移工具)

## 构建系统和依赖性管理工具

* [baur](https://github.com/simplesurance/baur) 只在一个 monorepos 分支中构建已更改的应用程序，并管理构建工件 ![github star](https://img.shields.io/github/stars/simplesurance/baur.svg?style=social&label=Star)
* [Bazel](https://bazel.build) 是谷歌的面向 monorepo 的构建系统。更多关于 Bazel 的信息：[awesome-bazel](https://github.com/jin/awesome-bazel) ![github star](https://img.shields.io/github/stars/jin/awesome-bazel.svg?style=social&label=Star)
* [Bit](https://github.com/teambit/bit) 是一个用于建立和管理具有多个组件的 JavaScript 项目的工具，并管理组件的依赖图。 ![github star](https://img.shields.io/github/stars/teambit/bit.svg?style=social&label=Star)
* [Bolt Pkg](https://github.com/boltpkg/bolt) 是一个超级强大的 JavaScript 项目管理。 ![github star](https://img.shields.io/github/stars/boltpkg/bolt.svg?style=social&label=Star)
* [Buck](https://buckbuild.com/) 是 Facebook 的面向 monorepo 的构建系统。 ![github star](https://img.shields.io/github/stars/facebook/buck.svg?style=social&label=Star)
* [drkns](https://github.com/frantzmiccoli/drkns) 是一个简单的、与语言无关的 monorepo 构建工具。 ![github star](https://img.shields.io/github/stars/frantzmiccoli/drkns.svg?style=social&label=Star)
* [Garment](https://github.com/Farfetch/garment) 是 Farfetch 的 monorepo 构建系统，具有集中和可定制的任务管理。 ![github star](https://img.shields.io/github/stars/Farfetch/garment.svg?style=social&label=Star)
* [GitLab CI](https://gitlab.com/gitlab-org/gitlab-ce/issues/19232) 11.4 支持根据路径变化执行相应的操作。
* [Lerna](https://lerna.js.org/) 是一个用于管理具有多个包的 JavaScript 项目的工具，建立在 Yarn 之上。 ![github star](https://img.shields.io/github/stars/lerna/lerna.svg?style=social&label=Star)
* [MBT](https://github.com/mbtproject/mbt) 是一个具有差异构建支持的构建工具。 ![github star](https://img.shields.io/github/stars/mbtproject/mbt.svg?style=social&label=Star)
* [Nix](https://github.com/NixOS/nix) 是一个具有远程缓存的软件包和发行版构建工具，主要由 NixOS 使用。 ![github star](https://img.shields.io/github/stars/NixOS/nix.svg?style=social&label=Star)
* [Nx](https://nx.dev/) 是一个用于 TypeScript monorepos 的构建系统和一套 monorepo 管理工具。 ![github star](https://img.shields.io/github/stars/nrwl/nx.svg?style=social&label=Star)
* [OAO](https://github.com/guigrpa/oao) 是一个基于 Yarn 的、有观点的 JavaScript monorepo 管理工具。 ![github star](https://img.shields.io/github/stars/guigrpa/oao.svg?style=social&label=Star)
* [Pants](http://www.pantsbuild.org/) 是一个面向 monorepo 的构建系统，被 Twitter、Foursquare 和其他多家公司使用。 ![github star](https://img.shields.io/github/stars/pantsbuild/pants.svg?style=social&label=Star)
* [Please](https://please.build/index.html) 一个跨语言的构建系统，强调高性能、可扩展性和可复制性。 ![github star](https://img.shields.io/github/stars/thought-machine/please.svg?style=social&label=Star)
* [pnpm](https://pnpm.js.org/en/) 是一个 JavaScript 依赖性管理工具，通过一组专门的命令 `pnpm multi` 来支持 monorepos。 ![github star](https://img.shields.io/github/stars/pnpm/pnpm.svg?style=social&label=Star)
* [Rush Stack](https://rushstack.io/) 是一个面向大规模TypeScript monorepos 的工具系列，以[Rush](https://rushjs.io/)构建协调器为基础。 ![github star](https://img.shields.io/github/stars/microsoft/rushstack.svg?style=social&label=Star)
* [Spago](https://github.com/spacchetti/spago) 是一个由Dhall和package-sets 支持的 PureScript 软件包管理器和构建工具。 ![github star](https://img.shields.io/github/stars/spacchetti/spago.svg?style=social&label=Star)
* [Symplify/MonorepoBuilder](https://github.com/Symplify/MonorepoBuilder) 是一个 PHP 的 monorepo 管理工具。 ![github star](https://img.shields.io/github/stars/Symplify/MonorepoBuilder.svg?style=social&label=Star)
* [Tainted](https://github.com/kynrai/tainted) 是一个确定哪些 Go 软件包需要在 monorepo 中重新构建的工具。 ![github star](https://img.shields.io/github/stars/kynrai/tainted.svg?style=social&label=Star)
* [Versio](https://github.com/chaaz/versio) 根据 [conventional commits](https://www.conventionalcommits.org/) 更新 monorepo 项目中的所有版本号，并可以生成更新日志和标签。 ![github star](https://img.shields.io/github/stars/chaaz/versio.svg?style=social&label=Star)
* [Yarn](https://yarnpkg.com/blog/2017/08/02/introducing-workspaces/) 是一个 JavaScript 依赖性管理工具，通过工作空间支持 monorepo。 ![github star](https://img.shields.io/github/stars/yarnpkg/yarn.svg?style=social&label=Star)
* [Layer-pack](https://github.com/layer-pack/layer-pack) 是一个 Webpack 插件，允许通过可继承的 npm 包/代码层和 es6 的 glob 导入来实现 monorepo 结构。 ![github star](https://img.shields.io/github/stars/layer-pack/layer-pack.svg?style=social&label=Star)

## 仓库管理工具

* [Builder](https://github.com/FormidableLabs/builder) 是一个工具，它使得在 Node.js monorepo 中的各个项目之间运送相同的脚本成为可能。例如，跨项目共享构建和测试脚本。 ![github star](https://img.shields.io/github/stars/FormidableLabs/builder.svg?style=social&label=Star)
* [FBShipIt](https://github.com/facebook/fbshipit) 是一个用 Hack 编写的库，用于将提交从一个仓库复制到另一个仓库。 ![github star](https://img.shields.io/github/stars/facebook/fbshipit.svg?style=social&label=Star)
* [adeira/shipit](https://github.com/adeira/shipit) 是 FBShipIt 的一个简化的 JavaScript 移植。 ![github star](https://img.shields.io/github/stars/adeira/shipit.svg?style=social&label=Star)
* [Lank](https://github.com/FormidableLabs/lank) 是一个在 Node.js monorepo 中使用自动配置 `NODE_PATH` 而不是符号链接将包链接在一起的工具。Lank 还允许你在所有（或所有）软件包的子集上运行相同的命令。 ![github star](https://img.shields.io/github/stars/FormidableLabs/lank.svg?style=social&label=Star)
* [monorepo-run](https://github.com/Akryum/monorepo-run) 是一个帮助程序的集合，用于在 yarn monorepo 的每个包中运行脚本，每个包有一个分离的窗格。 ![github star](https://img.shields.io/github/stars/Akryum/monorepo-run.svg?style=social&label=Star)
* [oao](https://github.com/guigrpa/oao) ![github star](https://img.shields.io/github/stars/guigrpa/oao.svg?style=social&label=Star)
* [Syncpack](https://github.com/JamieMason/syncpack) 允许在 Lerna Monorepos 中管理多个 package.json 文件。 ![github star](https://img.shields.io/github/stars/JamieMason/syncpack.svg?style=social&label=Star)
* [Ultra Runner](https://github.com/folke/ultra-runner) 是一个智能脚本运行器和 Lerna、Pnpm、Rush 和 Yarn 的构建工具。脚本同时运行，使用依赖性拓扑结构。构建过程会跟踪文件的变化，并在可能的情况下被跳过。 ![github star](https://img.shields.io/github/stars/folke/ultra-runner.svg?style=social&label=Star)
* [wsrun](https://github.com/whoeverest/wsrun) 允许在Yarn workspaces monorepo 的每个包中运行一个命令。 ![github star](https://img.shields.io/github/stars/whoeverest/wsrun.svg?style=social&label=Star)

## 一些好的参考文献

* [为什么谷歌将数十亿行代码存储在一个仓库中？](https://research.google.com/pubs/pub45424.html)
* [monorepo 的优势和劣势。谷歌的一个案例研究](https://dl.acm.org/doi/pdf/10.1145/3183519.3183550)
* [为什么你应该为你公司的所有项目使用一个单一的仓库？](https://www.drmaciver.com/2016/10/why-you-should-use-a-single-repository-for-all-your-companys-projects/)
* [monorepo 的优势](https://danluu.com/monorepo/)
* [Monorepos 使内心的源泉变得鲜活起来](https://kevingoslar.medium.com/monorepos-make-inner-source-come-to-life-bd1592b0cadf)
* [什么是 monorepo？(以及你应该使用它吗？)。](https://semaphoreci.com/blog/what-is-monorepo)
* [为 Semaphore-CI 用户提供 Monorepos 的持续集成。](https://semaphoreci.com/blog/continuous-integration-monorepos)

## 版本控制系统和附加组件

### Git

#### 工具

* [Git浅层克隆](https://git-scm.com/docs/git-clone) 让你只克隆部分的Git历史。
	* [如何使用 Git Shallow Clone 来提高性能](https://www.perforce.com/blog/git-beyond-basics-using-shallow-clones)
	* [如何用Git处理大的仓库](https://www.atlassian.com/blog/git/handle-big-repositories-git)
	* [Git克隆与浅层Git克隆](https://blogs.gnome.org/simos/2009/04/18/git-clones-vs-shallow-git-clones/)
* [Git filter-branch](https://git-scm.com/docs/git-filter-branch) 让你重写版本库的历史和修剪分支。
	* [如何用 Git 处理大型仓库](https://www.atlassian.com/blog/git/handle-big-repositories-git)
* [Git clone --single-branch](https://git-scm.com/docs/git-clone)
	* [如何用 Git 处理大型仓库](https://www.atlassian.com/blog/git/handle-big-repositories-git)
* [Git sparse-checkout](https://git-scm.com/docs/git-read-tree/)
	* [从 Git 克隆特定文件夹](https://lakehanne.github.io/git-sparse-checkout)
	* [如何用 Git 处理大型仓库](https://www.atlassian.com/blog/git/handle-big-repositories-git)
* [Git LFS](https://git-lfs.github.com/) 改善了 Git 中对大文件的处理。
* [GVFS](https://github.com/Microsoft/GVFS) 虚拟化你的 git repo 下面的文件系统，这样 git 和所有工具看到的似乎是一个正常的 repo，但 GVFS 只在需要时下载对象。仅适用 于Windows。 ![github star](https://img.shields.io/github/stars/Microsoft/GVFS.svg?style=social&label=Star)
* [SlothFS](https://gerrit.googlesource.com/gitfs/+/HEAD/docs/manual.md) 与 GVFS 类似，但只读。它在 Linux 和 macOS 上工作。
* [git subtree](https://github.com/apenwarr/git-subtree) 将你的项目中的子树合并和拆分到子项目中，然后再返回。从1.7版本开始成为 Git 的一部分。 ![github star](https://img.shields.io/github/stars/apenwarr/git-subtree.svg?style=social&label=Star)
    * [git subsplit](https://github.com/dflydev/git-subsplit) 自动并简化了管理单向只读子树分割的过程。 ![github star](https://img.shields.io/github/stars/dflydev/git-subsplit.svg?style=social&label=Star)
* [splitsh-lite](https://github.com/splitsh/lite) 是一个非常快速的 git subtree 替代品，可以将项目中的子树分割成子项目。 ![github star](https://img.shields.io/github/stars/splitsh/lite.svg?style=social&label=Star)
* [josh](https://github.com/esrlabs/josh) 是一个 git 服务器代理，可以实现仓库的即时虚拟化。 ![github star](https://img.shields.io/github/stars/esrlabs/josh.svg?style=social&label=Star)
* [go-diff](https://github.com/dstreamcloud/go-diff) 是一个方便的工具，可以分析哪些软件包由于变化而需要重建。 ![github star](https://img.shields.io/github/stars/dstreamcloud/go-diff.svg?style=social&label=Star)
* [mgt](https://github.com/nikita-skobov/monorepo-git-tools) 是一个工具，通过定义如何重新映射仓库的文件，使多个仓库之间的双向同步变得容易。 ![github star](https://img.shields.io/github/stars/nikita-skobov/monorepo-git-tools.svg?style=social&label=Star)

#### 扩展信息

* Atlassian 的 [Git 中的 Monorepos](https://developer.atlassian.com/blog/2015/10/monorepos-in-git/) 和[如何在 Git 中处理大的仓库](https://www.atlassian.com/blog/git/handle-big-repositories-git)涵盖了 Git 的扩展选项。

### Mercurial

#### 工具

* [Watchman](https://github.com/facebook/watchman)，当文件更改时，[fsmonitor](https://www.mercurial-scm.org/wiki/FsMonitorExtension) 将触发部分增量构建

#### 扩展信息

* [在 Facebook 扩展 Mercurial 的规模](https://code.facebook.com/posts/218678814984400/scaling-mercurial-at-facebook/)

## 开发流程工具

### Code reviews

* [Pull Review](https://github.com/imsky/pull-review/) Hubot 插件用于自动拉动评论，有很多配置选项。 ![github star](https://img.shields.io/github/stars/imsky/pull-review.svg?style=social&label=Star)
* [Rietveld](https://github.com/rietveld-codereview/rietveld) 是谷歌的一个代码审查工具，被 Chromium 使用。 ![github star](https://img.shields.io/github/stars/rietveld-codereview/rietveld.svg?style=social&label=Star)
* [API Extractor](https://api-extractor.com/) 是用来检测和审查 TypeScript 库的 API 签名的，也是用来发布多包 API 文档。 ![github star](https://img.shields.io/github/stars/microsoft/rushstack.svg?style=social&label=Star)

### CI 工具

* [在 Jenkins 中使用 Bazel 的增量 CI](https://www.kchodorow.com/blog/2015/10/15/one-weird-trick-for-fast-ci/)，文章作者 Kristina Chodorow（Bazel团队）。
* [bazel-travis](https://github.com/korfuri/bazel-travis) 这是一个在 Bazel monorepo 中使用 Travis CI 的最小设置。 ![github star](https://img.shields.io/github/stars/korfuri/bazel-travis.svg?style=social&label=Star)
* [buildpipe](https://github.com/jwplayer/buildpipe) 是一个通过观察项目的变化来动态生成 Buildkite 管道的工具。 ![github star](https://img.shields.io/github/stars/jwplayer/buildpipe.svg?style=social&label=Star)
* [Codefresh](https://codefresh.io/) 是一个针对 Docker/Kubernetes 的 CI/CD 平台，具有原生 [Monorepo 支持](https://codefresh.io/continuous-integration/using-codefresh-with-mono-repos/)。
* [使用 Monorepos 进行微服务的 CI/CD](http://blog.shippable.com/ci/cd-of-microservices-using-mono-repos) 这是一篇描述 Shippable.com 构建的文章，旨在触发特定于实际被修改的微服务和依赖于它的服务的构建。
* [Semaphore CI](https://semaphoreci.com) 是一个 CI/CD 平台，原生的 [monorepo 支持](https://docs.semaphoreci.com/essentials/building-monorepo-projects/)。

### Code ownership

* [GitHub's CODEOWNERS](https://help.github.com/articles/about-codeowners/) GitHub 的 CODEOWNERS 可以限制谁可以批准影响 monorepo 某一特定部分的 pull request。
* [Chromium 的 OWNERS 文件](https://chromium.googlesource.com/chromium/src/+/master/docs/code_reviews.md#OWNERS-files)启发了 GitHub 的 CODEOWNERS。
* [Write Guard](https://github.com/geritol/write-guard) 使用 GitHub 的 actions 来强制执行对 monorepo 项目的文件级写权限。
* [CODEOWNERS 生成器](https://github.com/gagoar/codeowners-generator) 从子文件夹中的文件为你的 monorepo 生成一个 CODEOWNERS 文件。

## 著名的公开 monorepos

* [Foursquare的开源项目](https://github.com/foursquare/fsqio) ![github star](https://img.shields.io/github/stars/foursquare/fsqio.svg?style=social&label=Star)
* [Stellar 的 Go monorepo](https://github.com/stellar/go) ![github star](https://img.shields.io/github/stars/stellar/go.svg?style=social&label=Star)
* [Habitat 的 monorepo](https://github.com/habitat-sh/habitat) ![github star](https://img.shields.io/github/stars/habitat-sh/habitat.svg?style=social&label=Star)
* [startup-os monorepo：谷歌开源工具（bazel等）在 monorepo 中的工作实例](https://github.com/google/startup-os) ![github star](https://img.shields.io/github/stars/google/startup-os.svg?style=social&label=Star)
* [M3 monorepo - 分布式TSDB，聚合器和查询引擎，Prometheus Sidecar，度量衡平台](https://github.com/m3db/m3) ![github star](https://img.shields.io/github/stars/m3db/m3.svg?style=social&label=Star)
* [Entria 的全栈式 Playground Monorepo](https://github.com/entria/entria-fullstack) ![github star](https://img.shields.io/github/stars/entria/entria-fullstack.svg?style=social&label=Star)
* [Berty 的 monorepo - React-native 移动应用程序 + Golang 后端 + Gomobile bridge + iOS & Android 原生驱动 + Protobuf](https://github.com/berty/berty/) ![github star](https://img.shields.io/github/stars/berty/berty.svg?style=social&label=Star)
* [NixOS 的软件包和模块的 monorepo 可用于增量构建和部署 Linux 机器。](https://github.com/NixOS/nixpkgs/) ![github star](https://img.shields.io/github/stars/NixOS/nixpkgs.svg?style=social&label=Star)
* [Celo 的 monorepo（包括区块链、杂项工具、库、操作东西诸如 terraform 模块、文档等）](https://github.com/celo-org/celo-monorepo)。 ![github star](https://img.shields.io/github/stars/celo-org/celo-monorepo.svg?style=social&label=Star)

## 迁移工具

* [Bazel 的 migration-tooling](https://github.com/bazelbuild/migration-tooling) 仓库。 ![github star](https://img.shields.io/github/stars/bazelbuild/migration-tooling.svg?style=social&label=Star)
* [Gazelle](https://github.com/bazelbuild/rules_go#generating-build-files) 为 Go 软件包自动生成 Bazel BUILD 文件。 ![github star](https://img.shields.io/github/stars/bazelbuild/rules_go.svg?style=social&label=Star)
* [tomono](https://github.com/unravelin/tomono) 将一组现有的Git仓库导入到一个单仓库中。 ![github star](https://img.shields.io/github/stars/unravelin/tomono.svg?style=social&label=Star)
* [shopsys/monorepo-tools](https://github.com/shopsys/monorepo-tools) 包含一套用于构建和拆分单体仓库的工具。 ![github star](https://img.shields.io/github/stars/shopsys/monorepo-tools.svg?style=social&label=Star)
* [Fastlane monorepo migration tools](https://github.com/fastlane/monorepo) 用于迁移代码和 github issues 的工具。专为 fastlane 设计，所以需要修改一些代码才能使用。 ![github star](https://img.shields.io/github/stars/fastlane/monorepo.svg?style=social&label=Star)

## 开发工作流

* [基于主干的开发](https://trunkbaseddevelopment.com)，是一种源码控制的分支模式，开发人员在被称为 "主干 "的单一分支上进行代码协作，通过采用文档技术，抵制任何创建其他长效开发分支的压力。因此，他们避免了合并地狱，不破坏构建，并从此幸福地生活在一起。
* [抽象的分支](https://www.branchbyabstraction.com)，是一个套路的技术，以实现树干的 "较长完成 "的变化。

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)]("http://creativecommons.org/publicdomain/zero/1.0/)

在法律允许的范围内，Uriel Corfa 已经放弃了本作品的所有版权和相关或邻近的权利。
