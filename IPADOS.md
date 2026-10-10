# iPadOS 17 播放器

本仓库是 [qist/tvbox](https://github.com/qist/tvbox) 的源配置 fork，本身不包含 iPad App。配套播放器是基于映匣修改的 [adolfheir/tvbox-silicon](https://github.com/adolfheir/tvbox-silicon)，iPhone / iPad 最低部署版本已调整为 17.0，并保留 JavaScript、DEX 和设备内 Java 插件运行时。

在播放器的设置中填入以下订阅地址，保存并更新：

```text
https://raw.githubusercontent.com/adolfheir/tvbox/master/fty.json
```

配置仍来自上游，未将第三方站点或插件改成自有服务；各源能否播放取决于网络、源服务和插件兼容性。

构建、侧载和测试范围见播放器的 [iPadOS 17 说明](https://github.com/adolfheir/tvbox-silicon/blob/main/Docs/IPADOS17.md)。截至 2026-10-10，完整设备版已编译通过，90 项核心测试通过，Mac 端已实测瓜子、光影和易听的播放进度；这些结果不等于 iPad 真机验收。连接的 iPadOS 17.7.11 设备仍须在设备上开启开发者模式，并注册到签名描述文件后，才能完成侧载及真机播放验收。

这是开发者侧载流程，不会提交到 App Store。
