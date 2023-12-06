<p align="center"><img alt="live.fanmingming.com" src="https://live.fanmingming.com/logo.png"></p>
<h1 align="center"> ✯ 一个可直连访问的电视/广播图标库与相关工具项目 ✯ </h1>
<h3 align="center">🔕 永久免费 直连访问 完整开源 不断完善的台标 支持IPv4/IPv6双栈访问 🔕</h3>

<p align="center">
<img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/fanmingming/live">
<img alt="GitHub forks" src="https://img.shields.io/github/forks/fanmingming/live">
<img alt="GitHub issues" src="https://img.shields.io/github/issues/fanmingming/live">
<img alt="GitHub watchers" src="https://img.shields.io/github/watchers/fanmingming/live">
<img alt="GitHub contributors" src="https://img.shields.io/github/contributors/fanmingming/live">
<img alt="GitHub" src="https://img.shields.io/github/license/fanmingming/live">
</p>

---

## 🤹‍♂️使用方法:

### 电视/广播图标库：
<table>
  <thead>
    <tr>
      <th>类 别</th>
      <th>调用路径</th>
      <th>图标数量</th>
      <th>更新时间</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>📺电视台图标库</td>
      <td><a href="https://github.com/fanmingming/live/tree/main/tv">https://live.fanmingming.com/tv/{频道名称}.png</a></td>
      <td>993个</td>
      <td>2023.12.5</td>
    </tr>
    <tr>
      <td>📻广播电台图标库</td>
      <td><a href="https://github.com/fanmingming/live/tree/main/radio">https://live.fanmingming.com/radio/{频道名称}.png</a></td>
      <td>465个</td>
      <td>2023.8.27</td>
    </tr>
  </tbody>
</table>

### 创建您的m3u订阅链接：
 - 下载 `demo.m3u` 空白示例文件并使用文本编辑软件打开。
   - https://live.fanmingming.com/tv/m3u/demo.m3u

 - 参考下方示例代码将`可用的CCTV1节目源`替换为您当地可用的直播源链接，依此类推逐个替换。
```
#EXTM3U x-tvg-url="https://live.fanmingming.com/e.xml"
#EXTINF:-1 tvg-id="CCTV1" tvg-name="CCTV1" tvg-logo="https://live.fanmingming.com/tv/CCTV1.png" group-title="央视",CCTV-1 综合
可用的CCTV1节目源
此处省略...
```
若您的直播源支持回看，请将第一行代码替换为：
```
#EXTM3U x-tvg-url="https://live.fanmingming.com/e.xml" catchup="append" catchup-source="?playseek=${(b)yyyyMMddHHmmss}-${(e)yyyyMMddHHmmss}"
```
 - 将编辑完成的m3u文件上传到您的Github仓库。
 - 为您的Github仓库开启Pages。
 - 通过播放器订阅您的m3u链接。

> 关于Github Pages：https://docs.github.com/en/enterprise-cloud@latest/pages/quickstart

## 🛠️工具
- 📆EPG接口地址：
  -  [https://live.fanmingming.com/e.xml](https://live.fanmingming.com/e.xml)
- 🏞️Bing每日图片：
  -  [https://fanmingming.com/bing](https://fanmingming.com/bing)
- 🎞️m3u8下载工具：
  -  [https://live.fanmingming.com/m3u8](https://live.fanmingming.com/m3u8)
- 📄M3U转TXT格式：
  - Demo🔗 [https://fanmingming.com/txt?url=https://live.fanmingming.com/tv/m3u/ipv6.m3u](https://fanmingming.com/txt?url=https://live.fanmingming.com/tv/m3u/ipv6.m3u)
- 🌐M3U8 Web Player:
  - Demo🔗 [https://live.fanmingming.com/player/?vurl=https://0472.org/hls/cctv13.m3u8](https://live.fanmingming.com/player/?vurl=https://0472.org/hls/cctv13.m3u8)

## 📖说明
- 项目EPG接口为112114.xyz站点分发，本项目无法确保其准确性。
- 通过M3U8 Web Player测试直播源需使用https协议的直播源链接。
- M3U转TXT格式工具构建在Vercel，不会记录您的访问日志请放心使用。
- 本项目不存储任何的流媒体内容，所有的法律责任与后果应由使用者自行承担。
- 您可以Fork本项目，但引用本项目内容到其他仓库的情况，务必要遵守开源协议。
- 项目m3u目录下的内容均收集于互联网，仅供测试研究使用，本项目不保证其有效性，也不再对相关issue做回复。
- 所有文件均托管在[GitHub](https://github.com/fanmingming/live)且自动构建，由项目发起人公益维护，欢迎Star本项目或点击[Issues](https://github.com/fanmingming/live/issues/new/choose)反馈您的问题。
- 您可以编辑本项目缺失的频道Logo到`tv`或`radio`目录下并发起拉取请求，收到请求后我们会对您提交的内容进行验证，审核通过后会自动发布。

## 📔更新
- 2023.12.05
  - 添加了一些电视频道台标。
