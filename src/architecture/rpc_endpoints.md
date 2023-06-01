# Solana 集群 RPC 端点

Solana 维护专用的 api 节点来满足每个公共集群的 JSON-RPC 请求，第三方也可以。以下是每个公共集群当前可用和推荐的公共 RPC 端点：

## Devnet 开发网

Endpoint 端点
    - https://api.devnet.solana.com - 单个 Solana 托管的 api 节点；限速

Rate Limits 速率限制
- 每个 IP 每 10 秒的最大请求数：100
- 单个 RPC 每个 IP 每 10 秒的最大请求数：40
- 每个 IP 的最大并发连接数：40
- 每个 IP 每 10 秒的最大连接速率：40
- 每 30 秒的最大数据量：100 MB

## Testnet 测试网

Endpoint 端点
    - https://api.testnet.solana.com - 单个 Solana 托管的 api 节点；限速

Rate Limits 速率限制

- Maximum number of requests per 10 seconds per IP: 100
- 每个 IP 每 10 秒的最大请求数：100
- Maximum number of requests per 10 seconds per IP for a single RPC: 40
- 单个 RPC 每个 IP 每 10 秒的最大请求数：40
- Maximum concurrent connections per IP: 40
- 每个 IP 的最大并发连接数：40
- Maximum connection rate per 10 seconds per IP: 40
- 每个 IP 每 10 秒的最大连接速率：40
- Maximum amount of data per 30 second: 100 MB
- 每 30 秒的最大数据量：100 MB

## Mainnet Beta 主网测试版

Endpoints* 端点*
    - https://api.mainnet-beta.solana.com - Solana 托管的 api
节点集群，由负载均衡器支持；限速

速率限制
- 每个 IP 每 10 秒的最大请求数：100
- 单个 RPC 每个 IP 每 10 秒的最大请求数：40
- 每个 IP 的最大并发连接数：40
- 每个 IP 每 10 秒的最大连接速率：40
- 每 30 秒的最大数据量：100 MB

*公共 RPC 端点不适用于生产应用程序。当您启动应用程序、删除 NFT 等时，请使用专用/私有 RPC 服务器。公共服务可能会被滥用，并且速率限制可能会更改，恕不另行通知。同样，高流量网站可能会被阻止，恕不另行通知。

## Common HTTP Error Codes 常见的 HTTP 错误代码

- 403 -- 您的 IP 地址或网站已被阻止。是时候运行您自己的 RPC 服务器或寻找私人服务了。
- 429 -- 您的 IP 地址超出了速率限制。减速！使用 Retry-After HTTP 响应标头来确定在发出另一个请求之前等待多长时间。
