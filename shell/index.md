
查看IP：
    ifconfig

查看当前文件/目录：
    ls -l 

显示隐藏文件：
    defaults write com.apple.finder AppleShowAllFiles Yes && killall Finder

不显示隐藏文件:
    defaults write com.apple.finder AppleShowAllFiles No && killall Finder

显示当前目录:
    pwd

创建文件夹：
    mkdir demo

创建文件：
    touch demo.js

查看当前文件夹里的所有文件（包括隐藏文件）：
    ls -ah


sudo xcode-select --switch /Users/dk/Downloads/Xcode.app/Contents/Developer

npm install -g cnpm --registry=https://registry.npm.taobao.org


查看当前使用的shell：
 echo $SHELL

查看系统所有shell：
 cat /etc/shells 

git bash自动补全功能：
brew install bash-completion

配置：
~/.bash_profile

if [ -f $(brew --prefix)/etc/bash_completion ]; then
     . $(brew --prefix)/etc/bash_completion
 fi

 执行：
source ~/.bash_profile

添加git自动补全

cd /usr/local/opt/bash-completion/etc/bash_completion.d
curl -L -O https://raw.github.com/git/git/master/contrib/completion/git-completion.bash
brew unlink bash-completion
brew link bash-completion


切换shell：
chsh -s /bin/zsh
chsh -s /bin/bash

https://sspai.com/post/55176


