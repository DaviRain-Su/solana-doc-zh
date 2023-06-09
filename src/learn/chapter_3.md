# Solana 钱包指南

本文档描述了 Solana 用户可以使用的不同钱包选项，这些用户希望能够在 Solana 区块链上发送、接收 SOL 代币并与之交互。

## 什么是钱包？


加密钱包是一种存储密钥集合的设备或应用程序，可用于发送、接收和跟踪加密货币的所有权。钱包可以有多种形式。钱包可能是计算机文件系统中的目录或文件、一张纸或称为硬件钱包的专用设备。还有各种智能手机应用程序和计算机程序提供了一种用户友好的方式来创建和管理钱包。

密钥对是安全生成的私钥及其加密派生的公钥。私钥及其对应的公钥一起称为密钥对。钱包包含一个或多个密钥对的集合，并提供一些与它们交互的方法。

公钥（通常简称为 pubkey）被称为钱包的接收地址或简称为地址。钱包地址可以自由分享和展示。当另一方要向钱包发送一定数量的加密货币时，他们需要知道钱包的接收地址。根据区块链的实施，该地址还可用于查看有关钱包的某些信息，例如查看余额，但无法更改钱包的任何信息或提取任何代币。

私钥需要对任何交易进行数字签名，以将加密货币发送到另一个地址或对钱包进行任何更改。绝不能共享私钥。如果有人获得了钱包私钥的访问权限，他们就可以提取其中包含的所有代币。如果钱包的私钥丢失，则发送到该钱包地址的任何代币都将永久丢失。

不同的钱包解决方案提供不同的密钥对安全方法、与密钥对交互以及签署交易以使用/花费代币。有些比其他的更容易使用。有些存储和备份私钥更安全。 Solana 支持多种类型的钱包，因此您可以在安全性和便利性之间做出适当的选择。

如果您希望能够在 Solana 区块链上接收 SOL 代币，您首先需要创建一个钱包。

## 支持的钱包

一些基于浏览器和移动应用程序的钱包支持 Solana。在 [Solana 生态系统](https://solana.com/ecosystem/explore?categories=wallet)页面上找到适合您的。

对于高级用户或开发人员，[命令行钱包](https://docs.solana.com/wallet-guide/cli)可能更合适，因为在集成到第三方解决方案之前，Solana 区块链上的新功能将始终首先在命令行上得到支持。
