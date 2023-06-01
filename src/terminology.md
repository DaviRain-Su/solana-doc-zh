# Terminology

以下术语在整个 Solana 文档和开发生态系统中使用。

## 账户


Solana 账本中的一条记录，它要么保存数据，要么是一个可执行程序。

与传统银行的账户一样，Solana 账户可能持有称为 [lamports]() 的资金。就像 Linux 中的文件一样，它可以通过密钥寻址，通常称为[公钥]()或公钥。

密钥可能是以下之一：
- 一个 ed25519 公钥
- 程序派生的帐户地址（32 字节值强制脱离 ed25519 曲线）
- 具有 32 个字符串的 ed25519 公钥的散列

## 帐户所有者

拥有该帐户的程序的地址。只有拥有程序才能修改帐户。


## app

与 Solana 集群交互的前端应用程序。

## bank 状态

在给定的[刻度]()高度解释分类账上所有程序的结果。它至少包括持有非零[原生代币]()的所有[账户]()的集合。


## block

[投票]()涵盖的分类账上的一组连续[条目]()。[领导者]()每个[时隙]()最多产生一个块。

## 区块哈希

标识记录（块）的唯一值（[散列]()）。 Solana 根据块的最后一个[条目 ID]() 计算块哈希。

## 区块高度


## 引导验证器


## BPF 加载器

## client

## commitment

## 集群

## compute budget 计算预算

## compute units 计算单元

## confirmation time 确认时间

## confirmed block 确认区块

## control plane 控制平面

## cooldown period 冷却时间

## credit 信用

## cross-program invocation (CPI) 跨程序调用（CPI）

## data plane 数据平面

## drone 无人机

## entry 进入

## entry id 条目编号

## epoch 纪元

## fee account 收费账户

## finality 终局性

## fork 叉子

## genesis block 创世块

## genesis config 创世配置

## hash 哈希

## inflation 通货膨胀

## inner instruction 内训


## instruction 指令

## keypair 密钥对

## lamport 灯口

## leader 领导者

## leader schedule 领导时间表

## ledger 账本

## ledger vote 账本投票

## light client 轻客户端


## loader 装载机

## lockout 停工

## message 留言

## native token 原生代币

## node 节点

## node count 节点数

## PoH PoH

## point 点

## private key 私钥

## program 程序

## program derived account (PDA) 程序衍生账户（PDA）

## program id 程序编号

## proof of history (PoH) 历史证明（PoH）

## prioritization fee 优先费

## public key (pubkey) 公钥（pubkey）

## rent 租金

## rent exempt 免租

## root 根

## runtime 运行时间

## Sealevel 海平面

## shred 切碎

## signature 签名

## skipped slot 跳过插槽

## slot 插槽

## smart contract 智能合约

## sol


## Solana Program Library (SPL) Solana 程序库（SPL）

## stake 赌注

## supermajority 绝大多数

## sysvar 系统变量

## thin client 瘦客户端

## tick 打勾

## tick height

## token 代币

## tps

## tpu

## transaction 交易

## transaction id 交易编号

## transaction confirmations 交易确认

## transactions entry 交易录入

## tvu 电视

## validator 验证器

## VDF


## verifiable delay function (VDF)

## vote 投票

## vote credit 投票相信

## wallet 钱包

## warmup period 热身期
