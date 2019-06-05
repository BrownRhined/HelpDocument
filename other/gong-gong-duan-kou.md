# 公共端口

## 概述  <a id="&#x6982;&#x8FF0;"></a>

公共端口与普通端口不同之处是允许多个用户使用同一个端口，而不是使用为每个用户单独分配的端口。

## 优势  <a id="&#x4F18;&#x52BF;"></a>

1. 某些组织或企业的内部网络可能有行为管理，并配置了端口限制。这时使用一般的配置就无法连接，使用公共端口则可以正常连接。
2. 某些运营商可能对非常用端口，特别是高位端口进行限速（因为高位端口多数被用于 BitTorrent）。使用常见端口可能对某些 ISP 的 QoS 有正面效果。

## 劣势  <a id="&#x52A3;&#x52BF;"></a>

1. 公共端口实现存在性能问题，使用此模式可能无法获得最佳性能。
2. 此模式可能容易出现 TCP 连接异常中断问题。
3. 此模式存在 UDP 性能问题。
