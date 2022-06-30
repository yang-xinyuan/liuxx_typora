neovim的配置文件处于

```shell
# windows 下的配置文件：

$ ~/AppData/Local/nvim/init.vim

# macos的配置文件的目录，默认下面的目录需要自己创建

$ ~/.config/nvim/init.vim
```



插件管理器

```shell
# mac
git clone --depth 1 https://github.com/wbthomason/packer.nvim\    ~/.local/share/nvim/site/pack/packer/start/packer.nvim
 
# windows 
git clone --depth 1 https://github.com/wbthomason/packer.nvim  "$env:LOCALAPPDATA\nvim-data\site\pack\packer\start\packer.nvim"
```



FiraCode字体安装

````shell
mac安装 FiraCode字体
```bash
brew tap homebrew/cask-fonts && brew install --cask font-fira-code-nerd-font
```
````

Iterm2 -> Preferences -> Profiles -> Text -> Non-Ascii-Font 选择 fira-code-nerd-font ,
之后重启 Iterm2 生效
