# V2和V3的池子差异？

V3是uniswap在2021年推出的新的AMM算法模型，直到2023年，PancakeSwap等交易所才开始采用。V3的模型采用“集中流动性”以提高资本利用率，用户在添加流动性的时候，可以自由选择价格区间，其操作难度和概念复杂度，比V2高了不少。

以下是V3资金池的特点：

### 1、V3池子不支持分红合约

和V2相比，V3不支持LP分红、持币分红等复杂的分红合约，只能支持标准合约。如果您在PandaTool创建的是分红合约，必须在V2添加流动性，以确保功能的稳定运行，不能在V3加池

### 2、V3锁池麻烦

很多人习惯通过Pinksales等平台锁池，一次锁个三年、五年的。但是V3的池子是无法这样锁的，至少在粉红平台并不支持，需要注意

### 3、Arb链不支持Uniswap V2

目前，Uniswap只在Arb链上部署V3合约。如果要想在Arb链上实现代币的复杂功能，需要通过SushiSwap V2做资金池

### 4、V3支持单边流动性

在一个成熟的资金池里，用户可以通过V3增加单边流动性，即只增加同一个代币，无需以交易对的形式添加流动性