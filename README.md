中国电信上海IPTV视频流地址列表
=======

注：这个播放列表使用IPTV的频道 **回放** 功能。IPTV直播用的是专网组播，无法直接通过Internet播放。<br>
因为不是所有频道都支持回放，所以这个列表里的频道 **必然少于** IPTV的直播频道。<br>
还有部分频道的回放地址播放错误，所以也没有收录。<br>
全部频道信息在excel文件里有记录，有需要的可以自己去查询。<br>


### 2018-4-22 IPTVplayseek.html功能更新

页面载入后默认以当前时间+延后4小时作为playseek参数添加，方便直接播放。由于时间输入框没有秒数，所以默认以0秒开始播放，相对实际时间会有延迟。

如果需要定时回放，可以手工设置开始和结束时间，使用“更新链接”按钮生成回放连接。注：只能回放前48小时的内容

也可以生成不带playseek参数的链接列表，考虑取消原来IPTV.htm的更新，用这个文件来取代。

另外还能生成m3u和txt文件的内容，以后这2个文件的内容也通过这个方式来更新。

### 2018-4-20 添加IPTVplayseek.html 可以自动添加playseek字串，方便播放

每次都要手工添加playseek，嫌麻烦，啃了些JS教程，写了这个页面。我的编程水平仅限于能给Excel写VBA，所以这个页面只能说大致能用，没做校验之类的设置，出错概率肯定很大，代码可读性也是一塌糊涂，大家多包涵。

如果有人能帮忙做些优化，感激不尽。

http://htmlpreview.github.com/?https://raw.githubusercontent.com/lucifersun/China-Telecom-ShangHai-IPTV-list/master/iptvplayseek.html

------
https://github.com/lucifersun/China-Telecom-ShangHai-IPTV-list/blob/master/IPTV.htm

部分视频源在Windows上用PotPlayer无法直接播放的，请加上`?playseek=YYYYMMDDhhmmss现在时间-YYYYMMDDhhmmss未来时间`即可播放。By:yangjuniori


------
### Kodi播放（PC版）

Kodi启用“电视”功能`(系统-电视-常规-启用)`，客户端使用“PVR IPTV Simple Client”，选择对应的m3u8列表文件，即可在主页面的“电视”内进行直播。

设置“后备帧率”为50Hz`(系统-电视-播放-后备帧率)`，可以播放所有频道。

Android版Kodi无法播放，建议利用网页列表选择频道+MXPlayer播放。

http://htmlpreview.github.com/?https://raw.githubusercontent.com/lucifersun/China-Telecom-ShangHai-IPTV-list/master/IPTV.htm

### iPhone/iPad播放

使用“小熊TV”，加载m3u8，可以正常播放所有频道。

https://itunes.apple.com/cn/app/小熊tv-免费高清电视直播-网络直播全聚合/id1069586855?mt=8

### 回放功能

RTSP链接后添加`?playseek=YYYYMMDDhhmmss-YYYYMMDDhhmmss`可以实现回放功能。By:ltycomputer
```
例:rtsp://124.75.34.37/PLTV/88888888/224/3221226230/10000100000000060000000000646848_0.smil?playseek=20160822203000-20160822210459
```
回放播放过程中拖动进度条会卡死，Windows(PotPlayer)与Android(MXPlayer)均有此现象。
