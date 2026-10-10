# iPadOS 17 播放器

本仓库是 [qist/tvbox](https://github.com/qist/tvbox) 的源配置 fork，本身不包含 iPad App。配套播放器是基于映匣修改的 [adolfheir/tvbox-silicon](https://github.com/adolfheir/tvbox-silicon)，iPhone / iPad 最低部署版本已调整为 17.0，并保留 JavaScript、DEX 和设备内 Java 插件运行时。

在播放器的设置中填入以下订阅地址，保存并更新：

```text
https://cdn.jsdelivr.net/gh/adolfheir/tvbox@master/fty.json
```

该地址通过 jsDelivr 提供本 fork 的 `fty.json`；连接的 iPad 访问 GitHub 原始域名超时，CDN 返回的内容已与仓库文件逐字节核对一致。配置仍来自上游，未将第三方站点或插件改成自有服务；各源能否播放取决于网络、源服务和插件兼容性。

构建、侧载和测试范围见播放器的 [iPadOS 17 说明](https://github.com/adolfheir/tvbox-silicon/blob/main/Docs/IPADOS17.md)。截至 2026-10-10，完整设备版已签名并安装到连接的 iPadOS 17.7.11 第六代 iPad，使用上述订阅已导入 48 个点播源和 6 份直播列表，瓜子真机播放已推进超过 53 秒并有正常视频画面；搜索已返回真实结果，但不能据此认定所有第三方源可用。光影当时选中的资源在真机上返回「无可用资源」，Mac 与模拟器的成功结果不能外推到真机。

这是开发者侧载流程，不会提交到 App Store。
