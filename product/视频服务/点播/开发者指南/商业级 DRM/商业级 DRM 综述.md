当前网络视频行业不断高速增长，网络盗版变得越发猖獗，给内容版权商也带来了非常大的损失，因此，内容版权保护的重要性不言而喻。

商业级 DRM 是一类基于播放许可证（License）实现高安全级别的内容版权保护解决方案。终端播放视频时，必须先获取 License（License 中包含了解密密钥、密钥有效期、终端信息等），然后使用 License 中的密钥解密播放视频。

使用商业级 DRM ，有如下优势：

<ul>
<li>密钥不可见：密钥本身被加密，仅内容解密模块（CDM）能读取密钥。</li>
<li>License 终端绑定：License 仅对单个终端有效，其他终端无法使用。</li>
<li>License 支持过期：支持指定 License 的有效期。</li>
<li>解码过程安全：支持硬件级（TEE）解密和解码。</li>
</ul>

目前主流的商业级 DRM 解决方案有 Widevine 和 FairPlay 两种：

| 商业级 DRM 解决方案 | 适用的自适应码流协议 | 适用播放环境                                        |
| ------------ | ---------- | --------------------------------------------- |
| Widevine     | HLS、DASH   | Andriod 播放器，以及 Chrome、Firefox、Edge、Opera 浏览器等 |
| FairPlay     | HLS        | iOS 播放器，以及 Safari 浏览器等                        |

目前点播支持两种 DRM 许可证服务集成方案：

- 云点播 DRM 集成方案：由腾讯云点播提供 DRM 许可证服务；
- 第三方 DRM 集成方案：由华曦达（SMDC）提供 DRM 许可证服务。

您可以根据需要，选择以上两种方案中的任意一种。

## 云点播 DRM 集成方案

商业级 DRM 能够为视频内容提供高级别的安全保障，但从零接入的门槛很高。因此，在此方案中，云点播提供了集成商业级 DRM 的一站式解决方案，包括 DRM 加密、证书管理、License 派发、解密播放等功能，帮助您轻松集成 DRM 能力。

加密和解密播放的整体架构流程图如下：
![](https://qcloudimg.tencent-cloud.cn/raw/416471d3730afc7449f3afd51ea9b5a8.png)

为了帮助您快速接入，我们为您提供了 [教程](https://cloud.tencent.com/document/product/266/79727)，以示例的方式为您讲解接入步骤。

## 第三方 DRM 集成方案

在此方案中，云点播提供转码、加密、存储、CDN 等功能，第三方 DRM 提供商（[华曦达 SDMC](https://www.xmediacloud.com/product-drm/)）提供证书管理、License 派发等功能。

加密和解密播放的整体架构流程图如下：

![](https://qcloudimg.tencent-cloud.cn/raw/abae964d9ee29cfcdcf6b9dc4c7e3dae.png)


为了帮助您快速接入，我们为您提供了 [教程](https://cloud.tencent.com/document/product/266/79730)，以示例的方式为您讲解接入步骤。

## 费用相关
使用商业级 DRM 加密，主要涉及以下费用：

- 转码费用：对视频进行 DRM 加密时，需要转码或转自适应码流，因此会产生转码费用。
- 存储费用：转码或转自适应码流的输出，会占用存储空间，因此会产生存储费用。
- DRM 许可证费用：终端播放 DRM 加密的视频时，需要获取 DRM 许可证，产生 DRM 许可证费用。如果使用第三方 DRM 集成方案，此项费用将由第三方 DRM 提供商收取。

以上费用的具体单价，请参见 [购买指南](https://intl.cloud.tencent.com/document/product/266/14666)。
