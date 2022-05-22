## 背景

由于最近学了vim，所以想用vim搭建一套java的开发环境

## 环境

neovim：是vim衍生出来的一个产品，它重写了vim底层的很多代码

SpaceVim：是vim与newvim的集成的IDE

python3：python3.x的版本即可，pythone2不支持

Jdk11

## 安装

### mac环境

1、安装neovim

```shell
$ brew install neovim
```

2、安装pythone环境

```shell
$ brew install python3
$ pip3 install neovim --upgrade
```

3、安装SpaceVIm

```shell
$ curl -sLf https://spacevim.org/cn/install.sh | bash
```

3、搭建java开发环境

https://github.com/eclipse/eclipse.jdt.ls

https://download.eclipse.org/jdtls/snapshots/?d







## 其他问题

1. Where should I put my configration?

SpaceVim load custom global configuration from ~/.SpaceVim.d/init.vim. It also support project specific configration, That means it will load .SpaceVim.d/init.vim from the root of your project.

2. E492: Not an editor command: ^M

The problem was git auto added ^M when cloning, solved by:

```source-shell
git config --global core.autocrlf input
```

3. Why SpaceVim can not display default colorscheme?

By default, SpaceVim use true colors, so you should make sure your terminal support true colors, This is an articl about what is true colors and the terminals which support true colors.

4. Why I can not update plugins?

Sometimes you will see Updating failed, The plugin dir is dirty. Since the dir of a plugin is a git repo, if the directory is dirty, you can not use git pull to update plugin. To fix this issue, just move your cursor to the error line, and press gf, then run git reset --hard HEAD or git checkout .. for more info, please read documentation of git.

5. How can I run the Python3 program?

已经向作者提交了issue，并且很快解决了，没看懂不要紧，要在mac 版本的SpaceVim上运行python3程序只需在行首加上#!python3,前提是你在命令行能使用python3命令，当然你写全路径也行，但是python3和!之间不能有空格

## 参考链接

https://www.jianshu.com/p/4e6dbc0aab50?utm_campaign=maleskine&utm_content=note&utm_medium=seo_notes&utm_source=recommendation