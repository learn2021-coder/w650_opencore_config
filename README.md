# w650_opencore_config
对应系统为Big Sur，wifi驱动也是对应的版本，如果想要安装在Monterey则要自己下载。
#### 电脑配置

- cpu:i7-7700
- gpu:mx150+hd630(独显被屏蔽)

#### ToDo

* [x] 加入蓝牙驱动,启动时间非常长,目前蓝牙未驱动
* [ ] 电池故障,电池未驱动  

#### 常用软件与配置:

- sudo spctl --master-disable
- Clashx: https://github.com/yichengchen/clashX
- Alfred: https://xclient.info/s/alfred.html#versions
- Moom: https://xclient.info/s/moom.html
- Homebrew: https://brew.sh
- Magnet: https://xclient.info/s/magnet.html
- Qtopencoreconfig: https://github.com/ic005k/QtOpenCoreConfig
- ohmyzsh: sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
- hidpi: https://github.com/xzhih/one-key-hidpi
- App Cleaner: https://freemacsoft.net/appcleaner/
- The unarchiver: https://theunarchiver.com/
-  Itlwm: https://github.com/OpenIntelWireless/itlwm
- Downie: https://xclient.info/s/downie.html
- Office : https://xclient.info/s/office-for-mac.html
- Typora: https://xclient.info/s/typora.html
- Dash: https://xclient.info/s/dash.html

> xcode-select --install 

> brew install  google-chrome telegram-desktop sublime-text visual-studio-code iterm2 karabiner-elements hackintool zsh zsh-syntax-highlighting zsh-autosuggestions uninstallpkg sogouinput  you-get yt-dlp mpv iina eudic 


#### 问题与解答  

1. xcrun: error 
> xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun  

> 解决方法  
> 重装xcode command line
> xcode-select --install
> 如果解决不了问题,执行一下命令
> sudo xcode-select -switch /

2. 任何源
> sudo spctl --master-disable

3. 交换option 和 command按键
> EFI/OC/kexts-voodooPS2Control.kext/contents/Plugins/voodooPs2keyboard.kext/contents/Info.plist/IOKitPersonalities/Platform Profile/Default/Swap command and option/YES

4. alfred最新版(tnt)不能用,改用旧版解决(新版已经解决）
5. 系统启动时间很长,根据代码发现是蓝牙驱动的问题,升级到特定的蓝牙驱动或者直接不加载蓝牙驱动(新驱动已经解决）
