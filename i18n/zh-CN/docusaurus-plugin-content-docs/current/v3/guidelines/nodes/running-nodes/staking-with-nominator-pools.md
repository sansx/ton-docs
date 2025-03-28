# 使用提名者池进行质押

## 概述

使用TON智能合约，您可以实现任何您想要的质押和存款机制。

然而，在TON区块链中存在“原生质押”——您可以将Toncoin借给验证者进行质押，并分享验证的奖励。

将Toncoin借给验证者的人称为**提名者**。

一个称为**提名者池**的智能合约，为一个或多个提名者提供了将Toncoin贷给验证者质押的能力，并确保验证者只能用该Toncoin进行验证。此外，智能合约保证了奖励的分配。

## 验证者与提名者

如果您熟悉加密货币，您一定听说过**验证者**和**提名者**。这些词经常出现在加密货币相关渠道中（我们的频道也不例外）。现在，是时候了解一下它们是什么了——区块链的两个主要参与者。

### 验证者

首先，让我们谈谈验证者。验证者是网络节点，通过验证（或确认）建议的区块并将其记录在区块链上来帮助维持区块链的运行。

要成为验证者，您必须满足两个要求：拥有高性能服务器并获得大量的TON（600,000）以进行质押。在撰写本文时，TON上有227个验证者。

### 提名者

:::info
提名者池的新版本已发布，更多信息请阅读单一提名者和归属合约页面。
:::

很明显，并不是每个人都能负担得起在余额上拥有100,000s的Toncoin——这就是提名者发挥作用的地方。简单来说，提名者是将其TON借给验证者的用户。每次验证者通过验证区块获得奖励时，奖励就会在参与者之间分配。

不久前，Ton Whales在TON上运行了第一个质押池，最低存款为50 TON。后来，TON基金会推出了第一个开放的提名者池。现在，用户可以以**10,000 TON**开始，以完全去中心化的方式质押Toncoin。

*来自[TON社区帖子](https://t.me/toncoin/543)。*

余额池应始终为 \*\*10  TON \*\* - 这是网络存储费的最低余额。

## 每月费用

由于验证轮次持续约 **18 小时**，每轮验证需要大约 **5 TON**，且一个提名池会参与奇数和偶数轮次的验证，因此运行该提名池每月大约需要 **105 TON**。

## 如何参与？

- [TON提名者池列表](https://tonvalidators.org/)

## 源代码

- [提名者池智能合约源代码](https://github.com/ton-blockchain/nominator-pool)

:::info
提名者的理论在[TON白皮书](https://docs.ton.org/ton.pdf)中有描述，章节2.6.3, 2.6.25。
:::
