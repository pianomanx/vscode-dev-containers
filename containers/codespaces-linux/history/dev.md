# [codespaces-linux](https://github.com/microsoft/vscode-dev-containers/tree/master/containers/codespaces-linux)
This document describes the base contents of the default GitHub Codespaces dev container image. Note that this image also includes detection logic to dynamically install additional language / runtime versions based on your repository's contents. Dynamically installed content can be found in sub-folders under `/opt`.

**Image version:** dev

**Source release/branch:** [master](https://github.com/microsoft/vscode-dev-containers/tree/master/containers/codespaces-linux)

**Digest:** sha256:eacd0cc5a18b19a4419571ea98d9615c241e140280c5a3b52476d82faa382314

**Tags:**
```
mcr.microsoft.com/vscode/devcontainers/universal:dev-focal
mcr.microsoft.com/vscode/devcontainers/universal:dev-linux
mcr.microsoft.com/vscode/devcontainers/universal:dev
```
> *To keep up to date, we recommend using partial version numbers. Use the major version number to get all non-breaking changes (e.g. `0-`) or major and minor to only get fixes (e.g. `0.200-`).*

**Linux distribution:** Ubuntu 20.04.2 LTS (debian-like distro)

**Available (non-root) user:** codespace

### Contents
**Languages and runtimes**

| Language / runtime | Version | Path |
|--------------------|---------|------|
| [Node.js](https://nodejs.org/en/) | 10.23.0<br />12.19.0<br />14.15.1 | /opt/nodejs/&lt;version&gt; |
| [Python](https://www.python.org/) | 3.6.12<br />3.7.9<br />3.8.6 | /opt/python/&lt;version&gt; |
| [Java](https://adoptopenjdk.net/) | 11.0.8 | /opt/java/&lt;version&gt; |
| [.NET](https://dotnet.microsoft.com/) | 2.1.814<br />3.1.407<br />5.0.202 | /home/codespaces/.dotnet<br />/opt/dotnet |
| [Ruby](https://www.ruby-lang.org/en/) | 2.7.2 | /opt/ruby/&lt;version&gt; |
| [PHP](https://xdebug.org/) | 7.2.34<br />7.3.27<br />7.4.16 | /opt/php/&lt;version&gt; |
| [PowerShell](https://docs.microsoft.com/en-us/powershell/) | 7.1.3 | /opt/microsoft/powershell |
| GCC | 9.3.0-17ubuntu1~20.04 | 
| Clang | 10.0.0-4ubuntu1 | 
| [Go](https://golang.org/dl) | 1.16.4 | /usr/local/go |
| [Rust](https://github.com/rust-lang/rust) | 1.52.1 | /usr/local/cargo<br />/usr/local/rustup |
| [Jekyll](https://jekyllrb.com/) | 4.2.0 | 

**Tools installed using git**

| Tool | Commit | Path |
|------|--------|------|
| [Oh My Zsh!](https://github.com/ohmyzsh/ohmyzsh) | d646884add277d134235a9b18ab755388d6e0d8d | /home/codespace/.oh-my-zsh |
| [nvm](https://github.com/nvm-sh/nvm.git) | 258938ef66a2a49a4a400554a6dce890226ae34c | /home/codespace/.nvm |
| [nvs](https://github.com/jasongin/nvs) | 780052d1e0b67a409b1382cd6e836cb39ca6188c | /home/codespace/.nvs |
| [rbenv](https://github.com/rbenv/rbenv.git) | 585ed84283f3308380b843391ee7b12706ecff87 | /usr/local/share/rbenv |
| [ruby-build](https://github.com/rbenv/ruby-build.git) | e9fa4bfdbe16b71964575eb8e1d27e348305d09b | /usr/local/share/ruby-build |

**Pip / pipx installed tools and packages**

| Tool / package | Version |
|----------------|---------|
| pylint | 2.8.2 |
| flake8 | 3.9.2 |
| autopep8 | 1.5.7 |
| black | 21.5b1 |
| yapf | 0.31.0 |
| mypy | 0.812 |
| pydocstyle | 6.1.1 |
| pycodestyle | 2.7.0 |
| bandit | 1.7.0 |
| virtualenv | 20.4.6 |
| pipx | 0.16.2.1 |

**Go tools and modules**

| Tool / module | Version |
|---------------|---------|
| golang.org/x/tools/gopls | 0.6.11 |
| honnef.co/go/tools | 0.1.3 |
| golang.org/x/lint | 0.0.0-20210508222113-6edffad5e616 |
| github.com/mgechev/revive | 1.0.6 |
| github.com/uudashr/gopkgs | 1.3.2 |
| github.com/ramya-rao-a/go-outline | 0.0.0-20200117021646-2a048b4510eb |
| github.com/go-delve/delve | 1.6.1 |
| github.com/golangci/golangci-lint | 1.40.1 |

**Ruby gems and tools**

| Tool / gem | Version |
|------------|---------|
| rake | 13.0.3 |
| ruby-debug-ide | 0.7.2 |
| debase | 0.2.4.1 |
| jekyll | 4.2.0 |

**Cargo / rustup (Rust) crates and tools**

| Tool / crate | Version |
|--------------|---------|
| rls | 1.41.0 |
| rustfmt | 1.4.36 |
| rust-analysis | 1.52.1 |
| rust-src | 1.52.1 |
| clippy | 1.52.1 |

**Other tools and utilities**

| Tool | Version | Path |
|------|---------|------|
| [git](https://github.com/git/git) | 2.31.1 | /usr/local |
| [Xdebug](https://xdebug.org/) | 3.0.4 | /opt/php/lts |
| [Composer](https://getcomposer.org/) | 2.0.8 | /opt/php-composer |
| [kubectl](https://github.com/kubernetes/kubectl) | 1.21.1 | /usr/local/bin |
| [Helm](https://github.com/helm/helm) | 3.5.4 | /usr/local/bin |
| [Docker Compose](https://github.com/docker/compose) | 1.29.2 | /usr/local/bin |
| [SDKMAN!](https://github.com/sdkman/sdkman-cli) | 5.11.4+709 | /usr/local/sdkman |
| [rvm](https://github.com/rvm/rvm) | 1.29.12 | /usr/local/rvm |
| [GitHub CLI](https://github.com/cli/cli) | 1.10.2 | 
| [yarn](https://yarnpkg.com/) | 1.22.10 | /opt/yarn |
| [Maven](https://maven.apache.org/) | 3.6.3 | /opt/maven |
| [Gradle](https://gradle.org/) | 7.0.2 | 
| Docker (Moby) CLI &amp; Engine | 20.10.6+azure | 

**Additional linux tools and packages**

| Tool / library | Version |
|----------------|---------|
| apt-transport-https | 2.0.5 |
| apt-utils | 2.0.5 |
| azure-cli (Azure CLI) | 2.23.0-1~focal |
| build-essential | 12.8ubuntu1.1 |
| ca-certificates | 20210119~20.04.1 |
| clang | 1:10.0-50~exp1 |
| cmake | 3.16.3-1ubuntu1 |
| cppcheck | 1.90-4build1 |
| curl | 7.68.0-1ubuntu2.5ppa1 |
| dialog | 1.3-20190808-1 |
| g++ | 4:9.3.0-1ubuntu2 |
| gcc | 4:9.3.0-1ubuntu2 |
| gdb | 9.2-0ubuntu1~20.04 |
| git | 1:2.25.1-1ubuntu3.1 |
| git-lfs (Git Large File Support) | 2.13.3 |
| gnupg2 | 2.2.19-3ubuntu2.1 |
| htop | 2.2.0-2build1 |
| iproute2 | 5.5.0-1ubuntu1 |
| iptables | 1.8.4-3ubuntu2 |
| jq | 1.6-1ubuntu0.20.04.1 |
| less | 551-1ubuntu0.1 |
| libatk-bridge2.0-0 | 2.34.2-0ubuntu2~20.04.1 |
| libatk1.0-0 | 2.35.1-1ubuntu2 |
| libc6 | 2.31-0ubuntu9.2 |
| libc6-dev | 2.31-0ubuntu9.2 |
| libcups2 | 2.3.1-9ubuntu1.1 |
| libgbm1 | 20.2.6-0ubuntu0.20.04.1 |
| libgcc1 | 1:10.2.0-5ubuntu1~20.04 |
| libgssapi-krb5-2 | 1.17-6ubuntu4.1 |
| libgtk-3-0 | 3.24.20-0ubuntu1 |
| libicu66 | 66.1-2ubuntu2 |
| libkrb5-3 | 1.17-6ubuntu4.1 |
| liblttng-ust0 | 2.11.0-1 |
| libnspr4 | 2:4.25-1 |
| libnss3 | 2:3.49.1-1ubuntu1.5 |
| libpango-1.0-0 | 1.44.7-2ubuntu4 |
| libpangocairo-1.0-0 | 1.44.7-2ubuntu4 |
| libsecret-1-dev | 0.20.3-0ubuntu1 |
| libssl1.1 | 1.1.1f-1ubuntu2.4 |
| libstdc++6 | 10.2.0-5ubuntu1~20.04 |
| libx11-6 | 2:1.6.9-2ubuntu1.1 |
| libx11-xcb1 | 2:1.6.9-2ubuntu1.1 |
| libxcomposite1 | 1:0.4.5-1 |
| libxdamage1 | 1:1.1.5-2 |
| libxfixes3 | 1:5.0.3-2 |
| lldb | 1:10.0-50~exp1 |
| llvm | 1:10.0-50~exp1 |
| locales | 2.31-0ubuntu9.2 |
| lsb-release | 11.1.0ubuntu2 |
| lsof | 4.93.2+dfsg-1ubuntu0.20.04.1 |
| lxc | 1:4.0.2-0ubuntu1 |
| make | 4.2.1-1.2 |
| man-db | 2.9.1-1 |
| manpages | 5.05-1 |
| manpages-dev | 5.05-1 |
| manpages-posix | 2013a-2 |
| manpages-posix-dev | 2013a-2 |
| moby-cli (Docker CLI) | 20.10.6+azure-1 |
| moby-engine (Docker Engine) | 20.10.6+azure-1 |
| nano | 4.8-1ubuntu1 |
| ncdu | 1.14.1-1 |
| net-tools | 1.60+git20180626.aebd88e-1ubuntu1 |
| openssh-client | 1:8.2p1-4ubuntu0.2 |
| openssh-server | 1:8.2p1-4ubuntu0.2 |
| pigz | 2.4-1 |
| pkg-config | 0.29.1-0ubuntu4 |
| procps | 2:3.3.16-1ubuntu2.1 |
| psmisc | 23.3-1 |
| python3-dev | 3.8.2-0ubuntu2 |
| python3-minimal | 3.8.2-0ubuntu2 |
| rsync | 3.1.3-8 |
| sed | 4.7-1 |
| software-properties-common | 0.98.9.5 |
| strace | 5.5-3ubuntu1 |
| sudo | 1.8.31-1ubuntu1.2 |
| tar | 1.30+dfsg-7ubuntu0.20.04.1 |
| unzip | 6.0-25ubuntu1 |
| valgrind | 1:3.15.0-1ubuntu9.1 |
| vim | 2:8.1.2269-1ubuntu5 |
| vim-doc | 2:8.1.2269-1ubuntu5 |
| vim-tiny | 2:8.1.2269-1ubuntu5 |
| wget | 1.20.3-1ubuntu1 |
| xtail | 2.1-6 |
| zip | 3.0-11build1 |
| zlib1g | 1:1.2.11.dfsg-2ubuntu1.2 |
| zsh | 5.8-3ubuntu1 |

