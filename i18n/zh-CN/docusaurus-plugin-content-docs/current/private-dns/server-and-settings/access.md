---
title: 权限设置
sidebar_position: 3
---

通过配置权限设置，可以保护 AdGuard DNS 免受未经授权的访问。 例如，您使用的是一个专用的 IPv4 地址，攻击者通过嗅探器识别了它，并向它发送大量请求。 没问题，只需将麻烦的域名或 IP 地址添加到列表中，它将不再打扰您！

被拦截的请求不会显示在查询日志中，也不会计入总请求限制。

## 设置方式

### 允许的客户端

此设置让用户指定哪些客户端可以使用您的 DNS 服务器。 它拥有最高优先级。 例如，如果同一 IP 地址同时在拒绝列表和允许列表中，它仍然会被允许。

### 禁止的客户端

在这里，用户可以列出不允许使用您的 DNS 服务器的客户端。 用户可以阻止所有客户端的访问权限，仅使用选定的客户端。 为此，将两个地址添加到不允许的客户端：`0.0.0.0/0` 和 `::/0`。 然后，在「_允许的客户端_」字段中，指定可以访问您服务器的地址。

:::note 重要信息

在应用访问权限设置之前，请确保没有阻止您自己的 IP 地址。 如果这样做，您将无法连接网络。 如果出现这种情况，只需断开与 DNS 服务器的连接，转到访问权限设置，并相应地调整配置。

:::

### 禁止的域名

这里可以指定将被拒绝访问 DNS 服务器的域名（以及通配符和 DNS 过滤规则）。

![其他设置 \*border](https://cdn.adtidy.org/content/release_notes/dns/v2-5/AS-en.png)

要在查询日志中显示与 DNS 请求相关联的 IP 地址，请选择「_记录 IP 地址_」复选框。 为此，请打开「_服务器设置_」→「_高级设置_」。