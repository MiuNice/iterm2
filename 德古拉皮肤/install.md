
*:@Author*: WangYH(Miu)


1. 从 git上下载 德古拉皮肤
```shell
git clone https://github.com/dracula/zsh.git
```
2. 将下载好的皮肤文件放到 ohmyzsh 皮肤目录下
```shell
cp zsh/dracula.zsh-theme ~/.oh-my-zsh/themes
```
3. 修改 ohmyzsh 皮肤
```shell
vim ~/.zshrc
# 将 ZSH_THEME 修改为 "dracula""

# 将 lib移动至 ~/.oh-my-zsh/themes/lib 下
cp -r zsh/lib ~/.oh-my-zsh/themes/lib

# 刷新 .zshrc
source ~/.zshrc
```
4. Iterm2 主题更改为 Dracula
```shell
# git clone 源码
git clone https://github.com/dracula/iterm.git
# 设置 itrem2 主题
1. iTerm2 > Preferences > Profiles > Colors > Color Presets > import
2. 选择 git clone 中 Dracula.itermcolors
3. 再次点击 Color Presets 选择 Dracula
```
5. 安装 插件
```shell
1. git 直接 clone 到 .zsh 目录下
# 自动补全 按“上” 则自动补全
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.zsh/zsh-autosuggestions
# 高亮显示命令
git clone https://github.com/zsh-users/zsh-syntax-highlighting ~/.zsh/zsh-syntax-highlighting

2. 离线安装（本目录下存在插件时）
# 自动补全 按“上” 则自动补全
cp -r zsh-autosuggestions ~/.zsh/zsh-autosuggestions
# 高亮显示命令
cp -r  ~/.zsh/zsh-syntax-highlighting

# 安装完成后 修改 ~/.zshrc
# 在文件末尾增加
source ~/.zsh/zsh-autosuggestions/zsh-autosuggestions.zsh
source ~/.zsh/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh

# 刷新 .zshrc
source ~/.zshrc
```


