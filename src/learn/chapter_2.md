# History

2017 年 11 月，Anatoly Yakovenko 发布了一份描述历史证明的白皮书，这是一种在互不信任的计算机之间保持时间的技术。从 Anatoly 之前在 Qualcomm、Mesosphere 和 Dropbox 设计分布式系统的经验来看，他知道可靠的时钟让网络同步变得非常简单。当同步很简单时，生成的网络可以非常快，仅受网络带宽的限制。

Anatoly 观察到没有时钟的区块链系统，如比特币和以太坊，在 Visa 等集中式支付系统需要 65,000 tps 的峰值时，难以在全球范围内扩展到每秒超过 15 笔交易。没有时钟，很明显他们永远不会毕业成为大多数人梦寐以求的全球支付系统或全球超级计算机。当 Anatoly 解决了让彼此不信任的计算机按时达成一致的问题时，他知道他掌握了将 40 年的分布式系统研究带入区块链世界的关键。由此产生的集群不会仅仅快 10 倍、100 倍或 1,000 倍，而是快 10,000 倍！

Anatoly 的实现始于私有代码库，并以 C 编程语言实现。 Greg Fitzgerald 曾在半导体巨头高通公司与 Anatoly 共事过，他鼓励他用 Rust 编程语言重新实现该项目。 Greg 曾从事 LLVM 编译器基础设施的工作，该基础设施是 Clang C/C++ 编译器和 Rust 编译器的基础。 Greg 声称该语言的安全保证将提高软件生产力，并且它没有垃圾收集器将使程序的性能与用 C 编写的程序一样好。Anatoly 试了一下，仅仅两周后，就将他的整个代码库迁移到了 Rust .卖。 Anatoly 计划将世界上所有的交易编织在一个单一的、可扩展的区块链上，并将该项目称为 Loom。

2018 年 2 月 13 日，Greg 开始制作 Anatoly 白皮书的第一个开源实现的原型。该项目在 loomprotocol 组织中以 Silk 的名称发布到 GitHub。 2 月 28 日，Greg 发布了他的第一个版本，证明可以在半秒多一点的时间内验证和处理 10,000 笔签名交易。不久之后，另一位前高通团队 Stephen Akridge 证明，可以通过将签名验证卸载到图形处理器来大幅提高吞吐量。 Anatoly 招募了 Greg、Stephen 和其他三人共同创立了一家公司，当时名为 Loom。

大约在同一时间，基于以太坊的项目 Loom Network 如雨后春笋般涌现，许多人对它们是否是同一个项目感到困惑。 Loom 团队决定重新命名。他们选择了 Solana 这个名字，这是对圣地亚哥北部一个名为 Solana Beach 的海滨小镇的致敬，Anatoly、Greg 和 Stephen 在 Qualcomm 工作期间曾在那里生活和冲浪了三年。 3 月 28 日，团队创建了 Solana GitHub 组织，并将 Greg 的原型 Silk 更名为 Solana。

2018 年 6 月，该团队将该技术扩展到在基于云的网络上运行，并于 7 月 19 日发布了一个 50 个节点、经过许可的公共测试网，持续支持每秒 250,000 笔交易的爆发。在 12 月发布的名为 v0.10 Pillbox 的后期版本中，该团队发布了一个在千兆网络上运行 150 个节点的许可测试网，并展示了浸泡测试平均每秒处理 20 万笔交易，突发交易超过 50 万笔。该项目还扩展到支持用 C 编程语言编写的链上程序，并在称为 SBF 的安全执行环境中同时运行。
