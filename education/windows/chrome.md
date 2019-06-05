---
description: 為 Chrome 配置 Shadowsocks 代理
---

# Chrome

 Chrome 浏览器搭配 [Proxy SwitchyOmega](https://switchyomega.com/) 扩展使用是非常方便的，此方案需要配合 Shadowsocks 客户端使用，并需要禁用 Shadowsocks 客户端的“启用系统代理”。



在开始下面的教程前的请确保 Shadowsocks 客户端已经配置好，如果没有请参考：

* 在 Windows 中配置 Shadowsocks 客户端
* 在 macOS 中配置 Shadowsocks 客户端

本教程不适用手机上的 Chrome 浏览器。

#### 安装 SwitchyOmega <a id="&#x5B89;&#x88C5;-switchyomega"></a>

通过 [Chrome 应用商店](https://chrome.google.com/webstore/detail/padekgcemlokbadohgkifijomclgjgif) 在线安装，如果无法访问，也可以从 Github [直接下载](https://github.com/FelisCatus/SwitchyOmega/releases)安装包

在 Chrome 地址栏输入 `chrome://extensions` 打开扩展程序，拖动 .crx 后缀的 SwitchyOmega 安装文件到扩展程序中按提示进行安装。

#### 配置 Shadowsocks 情景模式 <a id="&#x914D;&#x7F6E;-shadowsocks-&#x60C5;&#x666F;&#x6A21;&#x5F0F;"></a>

安装完成后会在 Chrome 浏览器右上角显示扩展程序的图标，如果你不想浏览器走代理可以选择“直接连接”，如图。

