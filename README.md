![](logo.png)


<!-- vim-markdown-toc GFM -->

- [目的](#目的)
- [基本规则](#基本规则)
- [如何参与?](#如何参与)
- [相关讨论](#相关讨论)
- [感谢](#感谢)

<!-- vim-markdown-toc -->

## 目的

1. 分享优秀的 vim 配置
2. 讨论 vim 配置技巧
3. 整理收集优秀的配置代码片段

## 基本规则

- 尽量使用 `nnoremap` 代理 `nmap`

`nmap` 是递归映射，如果映射的右边按键已经被映射为其他按键，那么将出现不可预期的问题。比如：

```vim
nmap j k
nmap k G
```

当按下 `j` 键时，实际上执行的是 `G` 键。


## 如何参与?

在 issue 列表里面留下你的 vimrc 配置链接。要求指定某一个 commit，避免后期推送影响阅读。

## 相关讨论

- [v2ex](https://www.v2ex.com/t/438522)

## 感谢

- 本仓库 Logo 来自 [vim-jp/reading-vimrc](https://github.com/vim-jp/reading-vimrc)

