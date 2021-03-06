# lx-music-desktop change log

All notable changes to this project will be documented in this file.

Project versioning adheres to [Semantic Versioning](http://semver.org/).
Commit convention is based on [Conventional Commits](http://conventionalcommits.org).
Change log format is based on [Keep a Changelog](http://keepachangelog.com/).

## [1.20.0](https://github.com/Haoqi7/luoxue-music/compare/v1.0) - 2022-05-10

特别说明：Scheme URL其实是支持Linux系统的，但好像需要deb之类的安装包创建出`.desktop`文件才行。

### 新增

- 新增播放详情页歌词右键菜单，原来设置-播放详情页设置的字体重置已迁移到此菜单内
- 新增歌词偏移设置，可以在播放详情页歌词右键菜单中使用
- 新增设置-播放设置-播放错误时自动切换歌曲设置，默认开启（原来的行为），若你不想在遇到音频加载失败、url获取失败等错误时自动切歌可以关闭此设置
- 新增设置-桌面歌词设置-自动刷新歌词置顶（当歌词置顶后仍被某些程序遮挡时可尝试启用此设置）
- 新增列表更新管理，可以在鼠标移入“我的列表”标题时出现的按钮中进入，这可以用来设置启动软件时需要自动从原平台更新的列表

### 优化

- 优化播放详情页背景显示，现在有背景图片的主题可以在播放详情页显示它的图片了
- 播放详情页在全屏状态下仍会显示退出播放详情页按钮，同时在其旁边添加退出全屏按钮
- 播放详情页在全屏状态下鼠标在空白处静止不动3秒后自动将其隐藏

### 修复

- 修复Linux无法全屏的问题
- 修复播放下载列表的歌曲时，使用Windows任务栏缩略图工具栏控制按钮的收藏按钮收藏歌曲时的异常问题
- 修复启用搜索历史但不启用热门搜索时，搜索历史不显示的问题
- 修复窗口尺寸设置对应的字体大小在启动后不生效的问题
- 修复wy源搜索某些歌曲时第一页之后的歌曲无法加载的问题
- 修复使用Scheme URL搜索歌曲时，不会自动关闭播放详情页（若处于打开状态）的问题
- 修复换源失败时的处理问题
- 修复启用代理时，https请求可能被挂起或被转为http的问题
- 修复正在下载的歌曲暂停任务后，再开始会导致程序卡死的问题

### 变更

- 播放详情页的任意地方右键双击隐藏详情页的行为，“任意区域”改为在“非歌词区域”

### 移除

- 移除设置-播放详情页设置-歌词字体重置，此设置项已迁移到播放详情页的歌词菜单中
- 移除播放详情页使用+-快捷键调整字体大小的功能，改用歌词右键菜单的字体大小调整功能