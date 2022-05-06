# 使用 Yaml 来管理 vimrc

- 讨论帖： #1
- 原始仓库：https://github.com/weirongxu/dotvim/tree/984a90298664e902eeb44eedc8081ac001002738

1. 安装方式以及载入逻辑的优化

原始的安装方式是，在 vimrc 里面加入相关代码，然后来 source vimrc.rc.vim, 这样的弊端在于，每次安装时都需要手动修改 vimrc，跨平台不易。在新版的vim中支持自动载入 `~/.vim/vimrc` （前提是没有 `~/.vimrc`）。

可以参考下 SpaceVim 初始载入的代码：

- https://github.com/SpaceVim/SpaceVim/blob/master/vimrc
- https://github.com/SpaceVim/SpaceVim/blob/master/init.vim

这是一个思路，就是利用了 vim neovim 自动载入配置的路径作为一个入口，然后同时重定向到一个主文件。
