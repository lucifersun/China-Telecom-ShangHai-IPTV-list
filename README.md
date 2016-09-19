##中国电信上海IPTV视频流地址列表##

https://github.com/lucifersun/China-Telecom-ShangHai-IPTV-list/blob/master/IPTV.htm

部分视频源在Windows上用PotPlayer无法播放，Android平台上用MXPlayer可以正常播放。

###Kodi播放###

Kodi启用“电视”功能`(系统-电视-常规-启用)`，客户端使用“PVR IPTV Simple Client”，选择对应的m3u8列表文件，即可在主页面的“电视”内进行直播。

设置“后备帧率”为50Hz`(系统-电视-播放-后备帧率)`，可以播放大部分PotPlayer无法播放的视频。`不知PotPlayer是否可以手动设置视频流的帧率？`

###回放功能###

RTSP链接后添加`?playseek=YYYYMMDDhhmmss-YYYYMMDDhhmmss`可以实现回放功能。By:ltycomputer
```
例:rtsp://124.75.34.37/PLTV/88888888/224/3221226230/10000100000000060000000000646848_0.smil?playseek=20160822203000-20160822210459
```
回放播放过程中拖动进度条会卡死，Windows(PotPlayer)与Android(MXPlayer)均有此现象。
