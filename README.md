# vim_peizhi
对vim进行个性化配置

# vim的配置文件
Vim的配置文件通常位于用户的主目录下，具体位置取决于操作系统和用户的配置。

在大多数Linux和Unix系统上，Vim的配置文件名为.vimrc，位于用户的主目录下。

# 1.下载 plug.vim 文件，根据操作系统不同，放置在以下autoload目录中：
Linux: ~/.vim/autoload
Windows: ~\vimfiles\autoload\plug.vim

plug.vim地址:https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim

# 2.目录结构如下，之后安装的插件将存放在plugged目录中：
如果没有~/.vim/autoload目录，使用 mkdir -p ~/.vim/autoload 创建即可。

# 3.在 ~/.vimrc 文件中增加plug-vim部分
在call plug#begin(‘~/.vim/plugged’) 与 call plug#end() 之间写上你需要的插件即可


# 4.在vim中执行命令。安装插件

安装插件 :PlugInstall 开始执行插件安装。
可以使用以下命令，指定安装特定的插件 :PlugInstall gist-vim
这里如果事macOS系统，提示“You have not agreed to the Xcode license agreements“
此时在终端输入 xcodebuild -license 同意xcode证书。

卸载插件 :PlugClean
先在vimrc配置文件中注释或者删除对应插件的配置信息，然后再执行命令

更新vim-plug插件自身 :PlugUpgrade
批量更新所有已安装的插件 :PlugUpdate

插件状态 :PlugStatus
使用该命令，可以查看当前已安装插件的状态信息


