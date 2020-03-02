# flash-player-without-help-service
老的Macromedia Flash播放插件，完美兼容IE11，不再有Help Service中国特供版锁区+强弹广告的烦恼！

众所周知adobe flash player中国版存在**锁区+强制弹广告+你删了广告就不让你用**的流氓行为，例如
http://tieba.baidu.com/p/5992864556

三种解决方案

* 都先卸载Adobe Flash Player和Flash Helper Service。大数字的软件管家可以清理干净，也可以手动卸载再去目录里删除

1. 使用旧版本的flash player
- 使用macromedia早年自带的flash player(被adobe买断之前)
- 早年有个exe版本，和flash MX 2004一起安装，我还没找到资源，有资源的老铁欢迎提issue或者mail rainydew@qq.com
- 我这里提供*fp_6.0.79_activex.exe*，直接双击安装，然后用IE11打开swf文件即可播放。可能会提示你插件未经确认，但不影响使用

2. 使用开源替代方案(均仅64位版本)
- ruffle，一个使用rust编写的flash播放器，可以在github找到。但官方仓库没有提供exe文件，在本仓库提供下载。在cmd下面 ruffle.exe 文件名.swf 即可播放
  - ruffle对于有些游戏处理的有bug，比如魔塔24层，囧
- lightspark，看起来更靠谱些的一个c++写的flash播放器，下载地址<https://github.com/lightspark/lightspark/releases>。但是我启动的时候提示gdi32.dll版本不正确……也许对你们有用
  - 好处是这是个界面程序……听说bug少一些，看官方仓库，开发也活跃一些

3. 使用独立版(debug版)
- 兼容性最好，本仓库也提供，没有发现广告
