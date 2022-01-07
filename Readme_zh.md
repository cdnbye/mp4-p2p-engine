**[English](README.md) | 简体中文**

<h1 align="center"><a href="" target="_blank" rel="noopener noreferrer"><img width="250" src="https://swarmcloud.net/logo.png" alt="cdnbye logo"></a></h1>
<h4 align="center">Save Your Bandwidth using WebRTC.</h4>
<h4 align="center">视频网站省流量&加速神器.</h4>
<p align="center">
  <a href="https://www.npmjs.com/package/cdnbye-mp4"><img src="https://img.shields.io/npm/v/cdnbye-mp4.svg?style=flat" alt="npm"></a>
  <a href="https://www.jsdelivr.com/package/npm/cdnbye-mp4"><img src="https://data.jsdelivr.com/v1/package/npm/cdnbye-mp4/badge" alt="jsdelivr"></a>
</p>

该项目处于实验节点，请考虑使用 [这个项目](https://github.com/swarm-cloud/mp4-sw-p2p-engine)替代。
<br>
mp4-p2p-engine 是一个 "简化版的Webtorrent"，只支持MP4格式，更小的体积，不需要磁力链接，极简的API，更高效的节点调度，简单而快乐！

## 优势
- 浏览器原生支持，不需要安装任何插件，采用仿BT算法，在线人数越多效果越好
- 支持基于MP4流媒体协议的点播场景
- 浏览器不支持WebRTC时无缝切换到HTTP下载模式
- 高可配置化，用户可以根据特定的使用环境调整各个参数
- 支持video.js、Clappr、Flowplayer、DPlayer等第三方播放器
- 通过有效的调度策略来保证用户的播放体验以及p2p率
- Tracker服务器根据访问IP的ISP、地域等进行智能调度

## 快速入门
将[quick-start.html](demo/quick-start.html)拷贝到您的网页中并运行。再打开另一个相同的网页。见证奇迹的时候到了！您已在两个网页之间建立了一个P2P连接，在不安装任何插件的情况下。如果在这个频道中（一个mpd标识了一个频道）没有其它参与者，那么您打开的第一个网页将作为种子为第二个网页提供数据。

## 浏览器支持情况
由于WebRTC已成为HTML5标准，目前大部分主流浏览器都已经支持。CDNBye的浏览器兼容性取决于WebRTC和[VideoStream](https://github.com/jhiesey/videostream)。需要注意的是iOS版Safari不支持MediaSource API。

兼容性|Chrome | Firefox | macOS Safari| 安卓微信/QQ | Opera | Edge | IE | iOS Safari | 
:-: | :-: | :-: | :-: | :-: | :-: | :-:| :-:| :-:
WebRTC Datachannel | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ❌ | ✔ |
VideoStream | ✔ | ❌ | ❌ | ✔ | ✔ | ✔ | ✔ | ❌ |
CDNBye | ✔ | ❌ | ❌ | ✔ | ✔ | ✔ | ❌ | ❌ | 

## 准备工作
如果MP4地址与网页不在同一个域，请确保流媒体服务器已做好跨域配置。
<br>
点击[这里](https://www.cdnbye.com/cn/views/mp4/usage.html#prepare)了解详情。

## 集成
通过script标签引入最新版本：
```html
<script src="https://cdn.jsdelivr.net/npm/cdnbye-mp4@latest"></script>
```

## API文档
参见 [API.md](https://www.cdnbye.com/cn/views/mp4/API.html)

## 后台管理系统
在接入P2P插件后，访问`https://www.cdnbye.com/oms`，注册并绑定域名，即可查看该域名的P2P流量、在线人数、用户地理分布等信息。

## 相关项目
- [hlsjs-p2p-engine](https://gitee.com/cdnbye/hlsjs-p2p-engine) - HLS协议的Web端P2P流媒体方案。
- [dashjs-p2p-engine](https://github.com/cdnbye/dashjs-p2p-engine) - MPEG-dash协议的Web端P2P流媒体方案。
- [shaka-p2p-engine](https://github.com/cdnbye/shaka-p2p-engine) - 同时支持HLS和Mpeg-Dash格式。

## FAQ
我们收集了一些[常见问题](https://www.cdnbye.com/cn/views/FAQ.html)。在报告issue之前请先查看一下。

## 联系我们
邮箱：service@cdnbye.com
