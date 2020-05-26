# vs code setting
vscode sncy setting


开启更多功能，提升办公效能

无标题
VSCode 安装和配置
由于VSCode性能强大，插件生态丰富，同时对团队内的主流语言和快捷键习惯都有良好的支持，因此目前团队首推的代码编辑器是VSCode。

下载和安装
访问官方网站 https://code.visualstudio.com/ 下载并安装

配置
如果你对VSCode的配置有自己的看法，可以按照自己的想法来配置，然而你如果希望使用一套在内部被广泛使用的，高效的，贴近Emacs快捷键风格的配置，可以按照下文的步骤来使用设置。

1. 安装 Setting Sync 插件
Setting Sync插件可以方便的同步其他人分享的配置，我们需要先安装他。
打开VSCode后在左边的图标列表中选择 extension ，并在搜索框中输入 setting sync ，并安装插件。

PS：安装结束需要按照提示重启VSCode



2. 使用 Setting Sync 来同步设置
安装了 Sync Setting 插件后，调出命令输入窗口（默认快捷键 Ctrl+Shift+P ），在其中输入 Sync ，并在下拉列表中选择 Sync:Advanced Options 一项


选择后，会出现新的可选项。选择其中的 Download Settings from public GIST 一项


选择后，sync插件会提示你类似「现在Sync插件将不再会要求你填写github token」之类的信息，代表其已经切换为使用public GIST 模式。

此时，再调出命令输入窗口，输入 Sync 并选择其中的 Download Settings 一项


并在出现的对话框中输入如下GIST id并回车：
a3129139103cd9eaa6019a8e7ebdc0e0

新版的 sync setting 可能会开启一个如下图的页面，此时需要点击图中位置的按钮 Download Public Gist 



此时插件会从gist https://gist.github.com/giyyapan/a3129139103cd9eaa6019a8e7ebdc0e0 中读取配置，并自动安装所需的插件，修改相应配置。

等同步结束后，VSCode 会改为使用一套在团队内部广泛使用的Emacs风格快捷键和插件集方案。

Emacs风格快捷键和默认的Windows风格快捷键有诸多不一致，入门可以参看《VSCode Emacs 快捷键》

3. 正确使用快捷键
为了最好的使用《VSCode Emacs 快捷键》中列出的快捷键，建议进行如下两个设置：

一，将 CapsLock 修改为 Ctrl
这将确保大部分的快捷键都可以比较轻松的按出来。

Ubuntu 18.04 系统下的安装方法：
首先安装 gnome-tweak-tool : sudo apt install gnome-tweak-tool
然后运行 gnome-tweak-tool 并进行如下修改


二，将搜狗(Fcitx)输入法中的冲突快捷键禁用掉
Fcitx输入法框架会占用很多快捷键位置（而且都是没有用的快捷键），和emacs风格键位，因此我们要把他们取消掉。
首先打开 Fcitx Configuration 程序

在 Global Config > Hotkey 中，将高级选项打开，浏览整个列表，将其中的快捷键全部取消掉（点击快捷键后按esc可以取消设置）
注意: 下面的 Show Advance Option 选项单选框选中后会多出很多选项，要滚动到底以确保所有快捷键都被清除（比如快捷键 Ctrl+Alt+p）



之后再点击到 Addon 一栏，依次双击打开每一个条目，将其中包括快捷键的地方全部清除掉。
 
一  阅

