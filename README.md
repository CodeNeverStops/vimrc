## 预览
![截图](https://cloud.githubusercontent.com/assets/322849/12638856/31df50ac-c5db-11e5-832c-57d4980811f4.png)

## 此配置适用于vim7.4

## 特性
- 完善的Golang开发环境，集成了代码高亮，自动完成等特性
- 集成Sublime Text molokai主题
- 使用Vundle.vim管理插件
- windows下使用Consolas和微软雅黑字体，需要导入font.reg到系统注册表中
- 按键集中在主键盘区域，摒弃恼人但需频繁使用的方向键
- 关闭了gvim的菜单栏和工具栏

## 使用方法
- 在系统的vimrc中加载本配置，例如: source $VIMRUNTIME/\_lvimrc
- 安装Vundle.vim插件来管理依赖的插件，安装完后，运行:PluginInstall来自动安装依赖的插件
- YouCompleteMe插件需要手动安装
- 复制go/bin目录下的预编译工具到$GOPATH/bin目录下

## 按键绑定
#### 普通模式
- ;wh 光标移动到左边的窗口
- ;wj 光标移动到下方的窗口
- ;wk 光标移动到上方的窗口
- ;wl 光标移动到右边的窗口
- ;tp 切换到前一个tab
- ;tn 切换到后一个tab
- ;tl 切换到最后一个tab
- ;tf 切换到第一个tab
- ;tc 关闭当前tab
- ;tm 移动当前tab到最后
- ;to 关闭所有tab，除了当前所在tab
- ;te :tabedit 命令缩写
- ;tt 两个tab之间切换
- ctrl+j 移动当前行到下一行
- ctrl+k 移动当前行到上一行

#### 可视模式
- ctrl+j 移动当前选中行（可以多行）移动到下一行
- ctrl+k 移动当前选中行（可以多行）移动到上一行
- gv 对当前选中字符串做vimgrep操作
- ;r 替换字符串缩写

#### 插入模式
- alt+h 向左移动光标
- alt+j 向下移动光标
- alt+k 向上移动光标
- alt+l 向右移动光标
- mac 下用command + h/j/k/l

#### 所有模式
- ;g vimgrep的缩写
- ;n 定位到vimgrep搜索出来的结果的下一个匹配项
- ;p 定位到vimgrep搜索出来的结果的上一个匹配项
- ;pp 关闭/打开复制模式

#### Go源文件按键绑定
- au FileType go nmap <leader>r <Plug>(go-run)
- au FileType go nmap <leader>b <Plug>(go-build)
- au FileType go nmap <leader>t <Plug>(go-test)
- au FileType go nmap <leader>c <Plug>(go-coverage)
- au FileType go nmap <Leader>ds <Plug>(go-def-split)
- au FileType go nmap <Leader>dv <Plug>(go-def-vertical)
- au FileType go nmap <Leader>dt <Plug>(go-def-tab)
- au FileType go nmap <Leader>dc <Plug>(go-doc)
- au FileType go nmap <Leader>dov <Plug>(go-doc-vertical)
- au FileType go nmap <Leader>db <Plug>(go-doc-browser)
- au FileType go nmap <Leader>im <Plug>(go-implements)
- au FileType go nmap <Leader>in <Plug>(go-info)

