**English | [简体中文](Readme_zh.md)**

<h1 align="center"><a href="" target="_blank" rel="noopener noreferrer"><img width="250" src="https://swarmcloud.net/logo.png" alt="cdnbye logo"></a></h1>
<h4 align="center">Let your viewers become your unlimitedly scalable CDN.</h4>
<p align="center">
  <a href="https://www.npmjs.com/package/cdnbye-mp4"><img src="https://img.shields.io/npm/v/cdnbye-mp4.svg?style=flat" alt="npm"></a>
  <a href="https://www.jsdelivr.com/package/npm/cdnbye-mp4"><img src="https://data.jsdelivr.com/v1/package/npm/cdnbye-mp4/badge" alt="jsdelivr"></a>
</p>

This projected is not production ready, please consider using [this](https://github.com/swarm-cloud/mp4-sw-p2p-engine).
<br>
mp4-p2p-engine is a "Simplified Webtorrent", only supports MP4, smaller size, no magnetic link, easier integrating, more efficient peers scheduling!

## Features
- WebRTC data channels for lightweight peer-to-peer communication with no plugins
- Support MP4 streaming
- Seamlessly fallback to normal server usage if a browser doesn't support WebRTC
- Highly configurable for users
- Support most popular HTML5 players such as video.js、Clappr、Flowplayer
- Efficient scheduling policies to enhance the performance of P2P streaming
- Use IP database to group up peers by ISP and regions

## Getting Started
Put the [quick-start.html](demo/quick-start.html) in your web page, run it. Wait for a few seconds，then open the same page from another browser. Now you have a direct P2P connection between two browsers without plugin!
The first web peer will serve as a seed, if no one else in the same channel.

## Browser Support
WebRTC has already been incorporated into the HTML5 standard and it is broadly deployed in modern browsers. The compatibility of CDNBye depends on the browser support of WebRTC and [VideoStream](https://github.com/jhiesey/videostream). Please note that iOS Safari "Mobile" does not support the MediaSource API.

Compatibility|Chrome | Firefox | macOS Safari| Android Wechat/QQ | Opera | Edge | IE | iOS Safari | 
:-: | :-: | :-: | :-: | :-: | :-: | :-:| :-:| :-:
WebRTC Datachannel | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ❌ | ✔ |
VideoStream | ✔ | ❌ | ❌ | ✔ | ✔ | ✔ | ✔ | ❌ |
CDNBye | ✔ | ❌ | ❌ | ✔ | ✔ | ✔ | ❌ | ❌ |

## Prepare
Make sure your file servers have proper CORS (Cross-origin resource sharing) headers so that data can be fetched across domain.
<br>
Click [here](https://www.hdtvcloud.com/en/views/mp4/usage.html#prepare) for more details.

## Include
Include the pre-built script of latest version: 
```html
<script src="https://cdn.jsdelivr.net/npm/cdnbye-mp4@latest"></script>
```

## API and Configuration
See [API.md](https://www.cdnbye.com/en/views/mp4/API.html)

## Console
Bind your domain in `https://oms.cdnbye.com`, where you can view p2p-related information.

## Related Projects
- [hlsjs-p2p-engine](https://github.com/cdnbye/hlsjs-p2p-engine) - Web Video Delivery Technology with No Plugins for hls.js.
- [dashjs-p2p-engine](https://github.com/cdnbye/dashjs-p2p-engine) - Web Video Delivery Technology with No Plugins for MPEG-dash.
- [shaka-p2p-engine](https://github.com/cdnbye/shaka-p2p-engine) - P2P engine for Shaka Player.

## FAQ
We have collected some [frequently asked questions](https://www.hdtvcloud.com/en/views/FAQ.html). Before reporting an issue, please search if the FAQ has the answer to your problem.

## Contact Us
Email: service@cdnbye.com
<br>
Telegram: @cdnbye
<br>
Skype: live:86755838




