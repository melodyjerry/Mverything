# Mverything
utools 插件, 用于在 Mac 平台下提供与 Windows 平台下 Everything 插件类似的搜索体验.
插件基于`mdfind`命令, `mdfind`命令基于 Spotlight 构建索引, 所以, 如果禁用了 Spotlight, 那么插件也将无法使用.
这可以被看做是 Spotlight 文件搜索的一个封装, 直接用 Spotlight 应该是相同的效果, 不过 all in one 总是舒服一点.

另外科普一下 Everything 是基于 NTFS 文件系统的特性实现实时搜索, Mac 无论如何也是很难达到 Everything 的速度的, 所以插件直接使用了『回合制搜索』(即输入完成后需要按一下回车再开始搜索)而不是『实时搜索』, 反正也做不到干脆放弃.

# 版本
- `0.0.5`
  1. 优化按键操作, 详情面板可通过`esc`键关闭并激活输入框, 左方向键可以也可以关闭详情面板
- `0.0.4`
  1. 增加文件详情面板
  2. 修改快捷键逻辑, 单击右方向键为打开文件详情, 双击右方向键用默认方式打开文件
  3. 修改升序降序按钮为图标
- `0.0.3`
  1. 增加操作提示说明板面
  2. 增加按照文件名, 大小等信息过滤的按钮
  3. 美化一些样式
- `0.0.2`
调整不和谐的样式(底部蓝条, 宽度过大导致出现滚动条)
- `0.0.1`
基本功能

# 下载
[下载最新版](https://github.com/lanyuanxiaoyao/Mverything/releases/latest)
[历史版本](https://github.com/lanyuanxiaoyao/Mverything/releases)

# 源码
没啥好敝帚自珍的.

传送门 → [Mverything](https://github.com/lanyuanxiaoyao/Mverything)

<div>
  <img alt="GitHub package.json version" src="https://img.shields.io/github/package-json/v/lanyuanxiaoyao/Mverything">
  <img alt="GitHub release version" src="https://img.shields.io/github/release/lanyuanxiaoyao/Mverything">
  <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/lanyuanxiaoyao/Mverything">
  <img alt="GitHub" src="https://img.shields.io/github/license/lanyuanxiaoyao/Mverything">
  <img alt="GitHub stars" src="https://img.shields.io/github/stars/lanyuanxiaoyao/Mverything">
</div>

# 操作
## 关键字
`find`, `查找`

## 基本操作
| 操作 | 功能 |
| --- | --- |
| `Enter(回车)` | 搜索 |
| `Arrow Right(右方向键单击)` | 文件详情 |
| `Arrow Right(右方向键双击)` | 默认方式打开文件 |
| `Mouse Left(鼠标左键双击)` | 默认方式打开文件 |
| `Mouse Right(鼠标右键单击)` | 快捷菜单 |

## 条件查询
目前支持几个简单的条件, 使用方式为`key:搜索词`

| 操作 | 功能 |
| --- | --- |
| `f` | 文件(即排除文件夹) |
| `F` | 文件夹(即排除文件) |
| `p` | 仅搜索图片文件(png, jpg, jpeg, ico, bmp, gif, psd, svg, tif, eps, raw) |

## 高级查询
所谓高级查询就是`mdfind`命令自己支持的一些高级查询, 如`mdfind "kMDItemContentType=public.folder"`, 但是平心而论, 这些关键字实在是...一言难尽, 所以这些高级用法大家自己去找吧.

# 截图

![安装界面](https://s2.ax1x.com/2019/08/08/eHPtb9.png)

![主界面](https://s2.ax1x.com/2019/08/08/eHPlCV.png)

![搜索界面](https://s2.ax1x.com/2019/08/08/eHCd1S.png)

![条件搜索](https://s2.ax1x.com/2019/08/08/eHP9AI.png)

![设置界面](https://s2.ax1x.com/2019/08/08/eHPZuQ.png)

![提示界面](https://s2.ax1x.com/2019/08/08/eHClOH.png)
