---
description: PandaTool新人发币教学
icon: layer-plus
---

# 新人发币必读

如果你是刚接触 “发币” 的小白用户，那恭喜你，看完这篇文章你就是发币专家了。

我们非常清楚，区块链领域的专业术语、多链差异、操作流程往往是你入门的最大障碍 —— 既不清楚 “发币” 究竟是创建代币还是搭建新链，也不知道该选 BSC 还是 Solana 链，更担心不会代码、怕平台有后门、发币后无法交易。

PandaTool将以最基础的概念开始，用通俗的语言拆解从 0 到 1 的完整发币流程。即便你是没有技术背景的新手，也能清晰掌握发币逻辑，避开常见陷阱，顺利完成代币创建与后续运营。

### **第一部分：发币前——知识与准备**

发币的前提是 “先懂逻辑，再备工具”，本部分正是为新手筑牢发币的 “基础防线”。只有先吃透这些知识、备齐工具，才能避免后续因概念混淆或工具缺失导致操作卡壳，为顺利发币做好铺垫。

#### **一、核心概念扫盲**

**1.什么是发币？**

* 就是在某条区块链上创建一个Token，这个代币的名称、数量全部由你来定义，你就是这个币的创始人。
* 注意，比特币那种是一条独立区块链，通过挖矿产出的POW公链，无法通过此方式创建。我们只是说，在某一条区块链上创建代币合约.

**2.在哪条链发币？**

* 这个是你需要提前思考好的。通常来说，有BSC（币安链.、ETH以太坊、Solana索拉拉.、TRON波场等区块链）。其中，BSC和Solana的热度比较高，不同链的功能、显示规则和成本不同。PandaTool 支持多条主流链（例如 BSC 与 Solana 热度较高）

<figure><img src="https://academy.pandatool.org/wp-content/uploads/2025/10/2025102407392592-1000x413.png" alt=""><figcaption></figcaption></figure>

**3.如何才能发币？**

* 正常情况下，发币需要一个程序员写代码，然后将代码部署到区块链上。如果你不会写代码，就可以借助像PandaTool这样的一键发币平台来完成。只需支付少量的服务费用，即可创建代币。

**4.发币平台有没有后门？**

* 发币平台赚的是服务费，即创建费用。每个人每创建一次代币，PandaTool都会收取相应的费用。这个费用是可持续的。既然有稳定的收入来源，为什么要安装后门自毁口碑？PandaTool的所有代码都是开源的，若有担忧，可自行审计合约代码。

**5.发币要付多少钱？**

* 不同区块链的发币费用不一样，通常以该链本身代币支付。例如你要在币安链发币，我们就收取BNB。你要在Solana链发币，我们就收取SOL。具体收多少？可以参考PandaTool的收费标准：[help.pandatool.org/price](https://help.pandatool.org/price)

**6.发了币之后能不能交易？**

* 只要为代币创建了流动性资金池（liquidity pool），就能交易。

**7.发的币能不能上币安、欧易？**

* 理论上不能，需要得到交易所的支持才可以。

**8.发的币能不能显示价格？**

* 部分平台支持显示（如 Ave、GMGN、Dextool），部分平台不支持，具体需咨询对应平台客服。

**9.发的币，能不能看到代币的头像、简介等？**

* 不同平台、钱包的规则不同 —— 部分可直接显示，部分需付费显示，部分不支持显示。

**10.我创建的代币能不能上GMGN、老鹰？**

* 当然可以，只要创建流动性并完成交易，GMGN、Ave、Dextool、老鹰 DexScreener 等平台均可查询到代币。

**11.我发的币，风险检测是不是全绿？会不会高风险？**

* 不同区块链、不同代币功能的风险各有不同。如果你特别在意风险这件事，那就不要创建功能代币，可以创建标准代币，风险检测全绿。因为只要带功能，就有可能有风险

**12.什么是内盘？这个和一键发币有什么不同？**

| **类型** | **资金池要求** | **代币归属**  | **功能机制** | **项目方掌控权** |
| ------ | --------- | --------- | -------- | ---------- |
| 内盘发币   | 无需创建资金池   | 需购买，无初始代币 | 无任何功能    | 基本无掌控权     |
| 一键发币   | 需手动创建资金池  | 全部进入自己钱包  | 可创建多功能   | 掌控权更大      |

* **内盘发币：**&#x53D1;币后不需要创建资金池，但是手里没有币，需要购买。而且内盘发币没有任何功能机制，项目方基本上没有掌控权
* **一键发币：**&#x53D1;币后代币全部进入自己的地址，但是需要手动创建资金池。项目方掌控权更大，可以创建不同功能的代播

目前PandaTool除了一键发币以外，也支持多个内盘发币：

* **PumpFun发币教程：**[https://help.pandatool.org/sol/createpump](https://help.pandatool.org/sol/createpump)
* **BonkFun发币教程：**[https://help.pandatool.org/sol/createbonk](https://help.pandatool.org/sol/createbonk)

**13.发的币权限在谁手里？怎么修改功能？**

有些代币有权限，有些没有（例如标准代币）。假设你创建的代币拥有权限，那么这个权限默认就是支付发币费用的钱包地址。通过我们的控制台或者权限管理工具，就可以使用这些权限，或者放弃权限。

<figure><img src="https://academy.pandatool.org/wp-content/uploads/2025/10/2025102407392641-1000x364.png" alt=""><figcaption></figcaption></figure>

* **BSC/ETH代币控制台：**[https://pandatool.org/#/coinrelease/console](https://pandatool.org/#/coinrelease/console)
* **Solana权限管理教程：**[https://help.pandatool.org/sol/control](https://help.pandatool.org/sol/control)
* **Sui权限管理教程：**[https://help.pandatool.org/sui/control](https://help.pandatool.org/sui/control)

#### **二、软/硬件准备**

在发币之前，我们要准备好一些硬件。所谓磨刀不误砍柴工，请准备好以下工具

* **电脑/手机：**&#x4E00;台电脑或者一部手机，这个是必须要有的。我们推荐使用电脑，苹果电脑或者Windows都可以。如果没有电脑，手机的话，苹果或者安卓机都行（尽量不要用华为.
* **科学软件：**&#x4E0D;管是手机还是电脑，都需要安装一个能够稳定访问谷歌等海外服务的软件，否则寸步难行
* **Telegram：**&#x8FD9;是必须要安装的，加入我们的官方Telegram交流群，才能为你解答问题

<figure><img src="https://academy.pandatool.org/wp-content/uploads/2025/10/2025102407392871.png" alt=""><figcaption></figcaption></figure>

* **钱包(软件/插件)：**&#x5982;果是电脑，需要安装谷歌浏览器，以及钱包插件，我们推荐小狐狸插件、OKX Web3钱包插件。如果是手机，我们推荐OKX钱包软件、TP钱包软件、小狐狸钱包软件等。
* **资产(代币)：**&#x94B1;包软件会生成钱包地址，钱包地址里要有相关的资产，以支付发币费用。例如你要在BSC链发币，钱包里至少得有0.06个BNB

总结下来就是:

* 如果你不会用钱包，不要发币
* 如果你钱包里没资产，不要发币
* 如果你不会科学上网，不要发币
* 如果你不知道发了币干什么，不要发币
* 如果你只用华为手机或者天天在微信宣传，不要发币

### **第二部分：发币中——操作与配置**

如果说 “发币前” 是 “打基础”，那么本部分就是 “落地实操” 的核心环节，带新手完成代币的 “从无到有”。同时，本部分还会给出 “按预算、需求、目标用户选链与功能” 的实用建议，让新手不仅会操作，还能做出符合自身项目的选择。

#### **一、基础参数设置**

* **全称：**&#x5C31;是这个代币的名称，例如Bitcoin/比特币这种，可以是中文、英文或者中英结合
* **简称：**&#x5C31;是这个代币的符号，例如BTC、ETH这种，可以是中文、英文或者中英结合
* **数量：**&#x4EE3;币的最大数量，通常在一亿亿以上。（数量是一次性到账，无法分批或者挖矿产出.
* **精度：**&#x4EE3;币的最小分割单位，直接默认即可（精度详细说明，参考文章 [https://blockweeks.com/docs/tech/decimals](https://blockweeks.com/docs/tech/decimals)）
* **头像：**&#x6709;些区块链可以传头像，如Solana。有些区块链不能传头像，如BSC。即便传了头像之后，也并不意味着会显示出来

以上就构成了代币的基本信息，接下来是一些高级参数

#### **二、高级功能解读**

* **增发功能：**&#x53EF;以随意增发代币，使得代币数量没有上限
* **黑名单功能：**&#x5F53;一个地址被加入到黑名单之后，这个地址将无法转出或者卖出代币
* **白名单功能：**&#x5F53;一个地址被加入到白名单之后，这个地址拥有豁免权限，例如可以豁免税率、豁免持仓限制等
* **销毁税：**&#x4EE3;币每交易一次，将有一部分的代币进入“黑洞地址”进行销毁，以此降低代币总量
* **营销税：**&#x4EE3;币每交易一次，营销钱包（项目方钱包.会获得一部分代币奖励
* **回流税：**&#x4EE3;币每交易一次，将有一部分代币被添加到流动性中，以扩大池子规模
* **最大持币量：**&#x4E00;个钱包地址最多可以持有多少代币，防止 “巨鲸” 控盘。
* **推荐奖励：**&#x4E24;个地址通过互相转账代币的方式完成上下级关系的绑定，上级可以获得下级交易的额外奖励
* **手动开启交易：**&#x521B;建流动性资金池后，需要手动打开此功能，代币才能进行交易，否则无法交易
* **自动空投：**&#x6BCF;产生一笔交易，就会将少量的代币空投到新的地址，以此增加持币地址数量
* **杀开盘机器人：**&#x5F00;启交易时，若检测到短时间内买入的地址，会判定为 “机器人” 并拉黑，防止机器人冲盘
* **标准代币：**&#x6CA1;有任何功能/税率/权限，就是一个纯粹的代币，风险检测全绿（教程：[标准代币 | PandaTool一键发币](https://help.pandatool.org/createtoken/stardand)）
* **持币分红：**&#x7528;户持有代币，即可获得另外一种代币的分红（如USDT、BNB等，教程：[持币暴力分红 | PandaTool一键发币](https://help.pandatool.org/createtoken/holdothers)）
* **多功能代币：**&#x53EF;以实现代币增发、暂停交易等多种功能（教程：[https://help.pandatool.org/createtoken/simplecontrol](https://help.pandatool.org/createtoken/simplecontrol)）
* **本币分红：**&#x7528;户持有代币，即可获得本币的分红（教程：[分红本币合约创建教程 | PandaTool一键发币](https://help.pandatool.org/createtoken/holdreflection)）
* **LP分红：**&#x6DFB;加流动性资金池成为LP的地址，可以额外获得代币奖励（一般是USDT或者BNB等,教程：[LP分红代币 | PandaTool一键发币](https://help.pandatool.org/createtoken/lpreflection)）
* **持币复利：**&#x7528;户持有代币，即可自动复利增发，使得余额越来越多（前几种分红来源于代币交易，复利来源于代币增发，教程：[持币复利+推荐奖励 | PandaTool一键发币](https://help.pandatool.org/createtoken/holdwithinviter)）
* **黑洞分红：**&#x7528;户将代币转入到黑洞地址销毁后，即可获得分红资格（教程：[黑洞分红教程 | PandaTool一键发币](https://help.pandatool.org/createtoken/blackhole)）
* 314协议：一个不通过Swap也能实现交易的代币合约（教程：[314协议发币教程 | PandaTool一键发币](https://help.pandatool.org/createtoken/314)）
* **Mint预售：**&#x7528;户将BNB或ETH转入到预售地址进行Mint，即可获得代币（项目启动前期筹集资金的一种方式，教程：[创建标准代币Mint预售教程 | PandaTool一键发币](https://help.pandatool.org/presale/simplemint)）
* **底池燃烧：**&#x6D41;动性资金池内每隔一段时间都会燃烧一部分代币，在池子内另一种代币（如USDT或BNB.不变的情况下，代币价格会自动上涨（教程：[底池燃烧 | PandaTool一键发币](https://help.pandatool.org/createtoken/lpburn)）
* **LP挖矿：**&#x7528;户添加流动性池成为LP之后，会获得挖矿奖励（教程：[LP挖矿+推荐奖励 | PandaTool一键发币](https://help.pandatool.org/createtoken/lpmine)）

&#x20;_再次强调，选择功能时请衡量合规与市场接受度：越复杂的功能越可能被风控类平台标记为“高风险”。如果你希望降低被屏蔽或提示风险的概率，建议优先选择**标准代币（无额外功能.）**。_

#### **三、不同区块链功能差异**

**1、EVM 系链（BSC、ETH、Base、X Layer 等）**

* 优势：功能最丰富，适合实现复杂合约逻辑；
* 劣势：成本与操作复杂度较高；
* 特殊规则：通常不直接支持头像显示

**2、Solana链**

* 优势：热度高；可设置头像；支持创建价格稳定的代币
* 劣势：功能简单，仅标准代币和转账税率 (Token2022) 两种机制
* 特殊规则：有黑名单、增发、更新代币资料等功能

**3、Sui链**

* 优势：可以设置头像；支持创建价格稳定的代币
* 劣势：只有一种代币，无法设置税率
* 特殊规则：有黑名单、增发、更新代币资料等功能

**4、TRON波场链**

* 优势：可以设置并修改头像、简介等
* 劣势：发币费用高；功能单一，目前只有标准代币
* 特殊规则：名称为网址、仿币、中文币等容易被屏蔽

<figure><img src="https://academy.pandatool.org/wp-content/uploads/2025/10/2025102407392994-1000x480.png" alt=""><figcaption></figcaption></figure>

**5、TON链**

* 优势：有头像
* 劣势：功能单一，只支持一种代币类型
* 特殊规则：可以增发、更新代币资料

#### **四、发币费用说明**

* 费用差异：不同区块链、不同功能的代币，发币费用不同
* 费用示例：最便宜的为 Polygon 链（20POL），最贵的为 BSC 链（0.05\~0.2BNB）
* 费用查询：详细收费列表可参考：[https://help.pandatool.org/price](https://help.pandatool.org/price)

#### **五、我该如何选择代币的功能、机制、区块链？**

我们无法准确告知大家，哪条区块链或者代币功能更加合适，只是从多个维度来分析一下：

* **区块链热度排序：**&#x42;SC＞Solana＞ETH＞波场＞X Layer＞Sui＞Base＞Polygon
* **操作难度排序：**&#x4C;P挖矿＞底池燃烧＞LP分红=黑洞分红=持币分红＞分红本币＞标准代币
* **综合操作成本排序：**&#x6CE2;场＞ETH＞Solana＞BSC＞Sui＞BASE＞X Layer＞Polygon

最终选择哪条区块链，需基于**预算**（成本承受能力）、**功能需求**（是否需要分红、增发等）、**目标用户群体**（用户常用链）综合决定。

### **第三部分：发币后——管理与常见问题**

发币并非 “创建完成即结束”，后续的代币管理、交易支持、问题排查，直接决定项目能否顺畅运行 —— 这正是本部分的核心价值。PandaToolo针对欧易提示恶意代码、波场链高风险、钱包链接失败等常见问题，给出具体解决办法，让新手在发币后也能应对自如。

#### **一、基础操作问题**

**1.发币后代币在什么地方？**

* 答：所有代币会进入 “创建代币时连接的钱包地址”。

**2.为什么我在钱包里没有看到代币？**

* 答：有些钱包不会直接显示代币，需要通过自定义添加代币的方式手动添加一下，可以看这个添加代币的教程：[钱包怎么添加代币？ | PandaTool一键发币](https://help.pandatool.org/question/addtoken)

<figure><img src="https://academy.pandatool.org/wp-content/uploads/2025/10/2025102407411595.png" alt=""><figcaption></figcaption></figure>

**3.发币后如何才能开源？验证合约代码？**

答：不同区块链对合约验证要求不同：

* Evms系（BSC、ETH、Base等），默认开源，无需操作
* X Layer区块链需要您手动开源，开源教程：[https://help.pandatool.org/question/xlayer-verified](https://help.pandatool.org/question/xlayer-verified)
* Solana链、Sui、Ton链暂时无需开源
* 波场链TRON需要手动开源，具体教程：[https://help.pandatool.org/tron/verify](https://help.pandatool.org/tron/verify)

**4.发币后如何才能交易？**

答：需要为代币创建一个流动性资金池，代币才能进行交易。不同区块链、不同交易平台，加池方式又有不同，可以详细阅读以下教程

* Solana加池教程：[https://help.pandatool.org/sol/creatpool](https://help.pandatool.org/sol/creatpool)
* BSC/ETH加池教程：[https://help.pandatool.org/createtoken/createliquidity](https://help.pandatool.org/createtoken/createliquidity)
* Sui加池教程：[https://help.pandatool.org/sui/pool](https://help.pandatool.org/sui/pool)

**5.不加池子可以转账吗？**

* 答：可以，代币间的转账功能并不依赖是否有资金池，随时都能转账。

**6.为什么代币检测有高风险？**

* 答：标准代币是不会有任何风险的。许多风控或托管平台基于合约权限、资金池规模、持币分布等多种规则判断风险，不同检测平台的检测逻辑不一样，复杂功能（如增发、黑名单）更容易被标记。例如，同一个代币，OKX检测没问题，币安检测就有问题。所以，如果大家比较在意风险的话，建议直接创建**标准代币**就可以。

<figure><img src="https://academy.pandatool.org/wp-content/uploads/2025/10/2025102407420219.png" alt=""><figcaption></figcaption></figure>

**7.为什么代币看不到头像logo？**

* 答：不同钱包、区块链、平台的显示规则不同：
  * **付费显示：**&#x90E8;分平台（如 Ave、TP 钱包）需付费才能显示；
  * **自动显示：**&#x90E8;分平台（如 OKX 钱包）可能会默认显示 Solana 链头像；
  * **手动上传：**&#x90E8;分区块链（如 BSC、ETH）需手动上传头像，并提供官网、社交媒体等资料审核；
  * **数据接入：**&#x90E8;分平台（如 PancakeSwap、Trust 钱包）会接入 CMC、CG 数据。
* 头像设置教程：
  * **付费提交 logo：**[https://pandatool.org/#/contractCheck/logo?lang=zh-CN](https://pandatool.org/#/contractCheck/logo?lang=zh-CN)；
  * **各平台上传教程：**[https://help.pandatool.org/question/logol](https://help.pandatool.org/question/logol)。

**8.为什么代币没有价格？**

答：价格显示由平台决定：

* 支持显示：创建资金池并交易后，Ave、Dextool、GMGN 等平台可显示价格；OKX 钱包可能显示价格；
* 不支持显示：TP 钱包等平台需满足 “高交易热度、多持币人数、大资金池” 才可能显示，无统一标准。

**9.我要为代币制作官网、白皮书吗？**

答：建议制作（若资金、技术允许）。成熟的代币项目需包含：官网、白皮书、Telegram 交流群、推特账号、Medium 博客、Discord。

* 进阶建议：
  * 联系审计公司获取代币审计报告；
  * 申请 CMC（CoinMarketCap）收录；
  * 申请 CG（CoinGecko）收录。

**10.我发的币，可以与我线下的产业、公司或者APP结合起来吗？**

* 答：具体得看结合的复杂度，总体来说不太可能。需要有专门的技术负责对接，同时代币本身也要合规才行。

**11.我发的币，可以在其他区块链使用吗？**

* 答：从技术上来说，可以实现，但需要构建一个跨链桥。通过跨链桥将代币从一条链跨到多个区块链上。如果没有跨链桥支持，那是不行的。

**12.我发了币之前，没有钱加池子、上头像，可以先预售吗？**

答：可以，预售本身就是用你的代币提前聚拢一部分资金，再通过这些资金去营销宣传代币。目前PandaTool提供三种预售工具，可以有针对的解决你的预售问题

* **标准预售教程：**[https://help.pandatool.org/presale/simplemint](https://help.pandatool.org/presale/simplemint)
* **加池预售教程：**[https://help.pandatool.org/presale/mintaddsale](https://help.pandatool.org/presale/mintaddsale)
* **捐赠预售教程：**[https://help.pandatool.org/presale/donatemint](https://help.pandatool.org/presale/donatemint)

#### **二、资金池专项问题**

**1.谁可以创建资金池吗？**

* 答：理论上，任何有代币的地址都可以创建，但一般来说是项目方自己创建。如果你启用了“手动开启交易”这个功能，那么除了项目方，别人无法创建。

**2.我创建了资金池之后，用户怎么交易呢？在哪里交易？**

* 答：一般来说，您在哪里创建的，用户去哪里交易。比如，BSC链的可以在PancakeSwap交易。ETH链的可以在Uniswap交易。Solana链的可以在Raydium交易等等。

**3.代币可以直接在OKX Web3钱包或者TP钱包的闪兑交易吗？**

* 答：不一定，钱包使用的是聚合DEX，仅支持符合其要求的代币（例：TP 闪兑、Phantom 内置 Swap 对代币有明确要求）。如果您的代币无法在某些钱包交易，可以咨询一下钱包客服。

**4.创建资金池需要投入多少资金？有没有最低标准？**

* 答：首次创建流动性资金池时，并不存在一个全网统一的“最低门槛”——理论上你可以只放很少的钱（例如几十美元.来创建池子。具体要放多少资金（如USDT、BNB、ETH等），完全取决于你的预算和项目目标，没有强制标准。

**5.那我投入的资金多或者少，有什么影响和区别吗？**

* 答：总的来说，投入的资金越多，可交易的代币数量就越多。
  * 投入 100USDT，用户单次可买 100\~200USDT 的代币；
  * 投入 10USDT，用户单次仅可买 10USDT 的代币。
* 参考链接：[https://academy.pandatool.org/zh\_CN/question/2008](https://academy.pandatool.org/zh_CN/question/2008)

**6.那有没有一种方式，投入资金少，但是用户可以买的多呢？**

答：正常情况下，池子内需要有对等金额的USDT，用户才能买入。但这种模式，在稳定池也可以实现。

如果是Solana区块链，可以通过创建CLMM稳定池的方式。只需通过“单币加池”的方式，添加您发行的土狗币，无需USDT这种价值币，也能让用户买入，这就实现了“小池子，大金额”的交易方式。

* CLMM稳定池创建工具：[https://solana.pandatool.org/createpool](https://solana.pandatool.org/createpool)
* CLMM稳定池创建教程：[https://help.pandatool.org/sol/clmm](https://help.pandatool.org/sol/clmm)

**7.创建资金池需要将代币加完吗？能不能预留？**

* 答：当然可以，假如您第一次创建流动性的时候，可以向流动性资金池内加入任意数量的代币（不能超过代币总量），无需全部进入流动性内。预留多少，完全凭自己的想法而定

**8.那池子里面的币会被买完吗？买完了怎么办？**

* 答：从资金池的合约逻辑来看，“池子里的币被买完”的情况不会出现。池子里的代币会随着买入减少，但价格会逐步升高。于是，池子里的代币无限趋近于0，代币价格不断上涨，趋近于无穷大。所以，池子代币数量不会完全变成0，只是会慢慢减少。而且随着代币价格越来越高，能买到的代币数量也会越来越少。如果想增加池子里的代币数量，可以通过增加流动性的方式实现。
* 重要提醒：不可直接向池子地址转账代币，否则会导致资金池内 USDT 被掏空。

**9.投入资金池的钱能不能取回来？**

* 答：创建流动性池时，你会获得一个 LP（流动性凭证）代币，代表你在池中的份额。 只要你没有销毁这个 LP 代币，就可以随时将资金池内的代币撤出。但具体能撤出多少，取决于当前池子内有多少币。

**10.别人买我的代币，钱去了哪里？是直接到我的地址吗？**

答：不是。别人购买你的代币，是把钱放到资金池里。然后资金池给他代币。如果是卖币，就是把币放到资金池里，资金池给他钱。所以，整个流程是依托于资金池运行的。如果你想获得用户买币的钱，将资金池撤了就可以。

* 用户买币：将钱转入资金池，资金池向用户发放代币；
* 用户卖币：将币转入资金池，资金池向用户发放钱；
* 项目方收款：需撤出资金池才能获得用户买币的资金。
* 详细教程：[https://academy.pandatool.org/zh\_CN/kn/805](https://academy.pandatool.org/zh_CN/kn/805)

**11.别人买我的代币后，我能冻结让他不能卖吗？**

* 答：如果你发行的代币拥有黑名单功能，就可以实现。但是这种功能具有较高的危险性，拥有该功能的代币可能会被检测为高风险代币

**12.代币价格是怎么定的？**

答：代币初始价格（发行价.由第一次加池的比例决定。如果你加100U和100个币，那么代币的上线价格就是1U。如果你加100U和10000个币，代币的上线价格就是0.01U，以此类推

* 加 100USDT+100 个币，初始价格 = 1USDT / 个；
* 加 100USDT+10000 个币，初始价格 = 0.01USDT / 个。

价格涨跌只与买卖有关。当买盘大于卖盘，价格上涨，反之下跌。简单来说，买的越多价格越涨，卖的越多价格越跌

**13.那代币价格能固定吗？**

答：通过创建稳定池，可以让代币的价格在一个较小的范围内波动，从而实现价格的相对稳定。目前，PandaTool支持Solana和Sui链创建稳定池：

* Sui稳定池工具：[https://help.pandatool.org/sui/pool](https://help.pandatool.org/sui/pool)
* Solana稳定池工具：[https://help.pandatool.org/sol/clmm](https://help.pandatool.org/sol/clmm)

14.**听说Solana创建资金池需要市场ID？是这样吗？**

答：不完全是这样。Solana区块链上面有三种资金池类型，分别是AMM、CPMM和CLMM。这三个，仅 AMM 需要市场 ID（创建 AMM 前需先创建市场 ID，且需支付成本）如果你不想出这个费用，可以选择CPMM和CLMM创建，三种资金池的区别，可以参考下面的教程

* Solana资金池区别：[https://academy.pandatool.org/zh\_CN/question/217](https://academy.pandatool.org/zh_CN/question/217)

**15.那到底什么是市场ID呢？**

答：Openbook Market ID是一个独特的ID，允许您的代币在defi平台上进行交易。通过这个ID，各大交易平台可以识别到你的流动性，所以一个ID只能用来对应一个交易对（如USDT/SOL）。属于历史产品，非必需操作。

* 市场ID创建工具：[https://solana.pandatool.org/market](https://solana.pandatool.org/market)
* 市场ID创建教程：[https://help.pandatool.org/sol/market](https://help.pandatool.org/sol/market)

**16.当我为代币创建了流动性资金池之后，在哪里可以看到？**

答：如果你是在PandaTool创建的流动性，PandaTool是支持查看的。进入流动性管理页面，连接钱包就能看到你的资金池了

* BSC/ETH流动性控制台：[https://pandatool.org/#/LPmanage?lang=zh-CN](https://pandatool.org/#/LPmanage?lang=zh-CN)
* Solana流动性管理：[https://solana.pandatool.org/managepool](https://solana.pandatool.org/managepool)
* Sui链流动性管理：[https://sui.pandatool.org/liquidity/manage](https://sui.pandatool.org/liquidity/manage)

<figure><img src="https://academy.pandatool.org/wp-content/uploads/2025/10/2025102407435266.png" alt=""><figcaption></figcaption></figure>

15.**为什么我已经创建了资金池，但是交易代币的时候还提示流动性不足？**

答：通常来说，流动性不足有两个原因：

1. DEX 不支持该流动性（例：OKX 钱包聚合 DEX 不支持部分池子）；
2. 交易数量大于资金池内代币数量，需增加流动性或降低交易金额。

16.我创建的流动性是BNB或者ETH交易对，可以用USDT购买吗？

* 答：没有问题，流动性资金池会自动将USDT换成BNB或ETH存在资金池里面的，所以无需担心，随意兑换

#### **三、常用工具解读**

除了发币之外，PandaTool 提供多种发币后辅助工具，覆盖转账、控盘、流动性管理等场景：

**1.如何将代币批量转账给多个地址？一笔笔转太麻烦了**

答：如果你想将代币一次性空投给多个地址，就可以使用PandaTool的**批量转账**工具。BSC链一次支持批量转账200个地址，可以彻底解放双方，实现多地址快速转账。

* BSC/ETH批量转账教程：[https://help.pandatool.org/tools/batch-transfer](https://help.pandatool.org/tools/batch-transfer)
* Solana批量转账教程：[https://help.pandatool.org/sol/batch-transfer](https://help.pandatool.org/sol/batch-transfer)

**2.我想将代币批量空投给USDT的持币地址，但如何知道是哪些地址呢？**

答：针对该问题，PandaTool开发了**代币快照**工具，可以获得某一个代币的持仓地址。例如你输入USDT，就能导出USDT的持仓地址。再通过这些地址，就能进行批量转账了。

* BSC/ETH代币快照教程：[https://help.pandatool.org/tools/snapshottoken](https://help.pandatool.org/tools/snapshottoken)
* Solana代币快照教程：[https://help.pandatool.org/sol/snapshottoken](https://help.pandatool.org/sol/snapshottoken)

**3.我创建了资金池后，能否通过多个地址来实现代币拉盘/砸盘，以达到控盘的目的呢？**

答：当然可以，PandaTool开发了针对不同区块链的**市值管理工具**，可以让你一次性导入数十个或者数百个地址，通过这些地址的买卖来实现代币的价格涨跌，从而在一定程度上达到控盘的目的。

* EVM市值管理（支持BSC、Base、ETH等）教程：[https://help.pandatool.org/createtoken/swapbot](https://help.pandatool.org/createtoken/swapbot)
* Solana市值管理教程：[https://help.pandatool.org/sol/swapbot](https://help.pandatool.org/sol/swapbot)
* 波场市值管理教程：[https://help.pandatool.org/tron/trxbot](https://help.pandatool.org/tron/trxbot)

<figure><img src="https://academy.pandatool.org/wp-content/uploads/2025/10/2025102407445232-1000x548.png" alt=""><figcaption></figcaption></figure>

**4.但是我们没有这么多钱包地址怎么办呢？一个个搞太麻烦了**

答：为此，PandaTool开发的**批量生成钱包**工具，支持在几秒内生成数百个地址，包括波场地址、以太坊地址、Solana地址等，非常方便。当这些钱包生成之前，你再通过批量转账工具，将代币转进去，就可以用市值管理操盘了

* BSC/波场钱包创建教程：[https://help.pandatool.org/tools/create-wallets](https://help.pandatool.org/tools/create-wallets)
* Solana钱包创建教程：[https://help.pandatool.org/sol/createwallet](https://help.pandatool.org/sol/createwallet)

**5.这些钱包可以是靓号钱包吗？例如带888这种尾号的钱包地址？**

答：PandaTool目前支持创建Solana靓号钱包，可以自定义钱包的开头前缀和尾号，这样就是靓号地址了

* Solana靓号钱包生成教程：https://help.pandatool.org/sol/vanityAddress

**6.当我用完市值管理之后，如何将这些钱包内的币归集到一起？**

答：可以使用PandaTool的批量归集工具，通过导入钱包私钥，即可一次性归集多个钱包内的多种代币。

* BSC/ETH批量归集教程：[https://help.pandatool.org/tools/gather](https://help.pandatool.org/tools/gather)
* Solana批量归集教程：[https://help.pandatool.org/sol/gather](https://help.pandatool.org/sol/gather)

**7.有用户反馈，说我的项目池子太小了，我该如何增加池子？**

答：切记，池子小的话，不能直接往池子里转账代币。需要通过PandaTool的流动性管理工具来完成，支持增加流动性。当然，如果你想移除流动性，也可以在这里实现。

* BSC/ETH增加与撤出流动性：[https://help.pandatool.org/createtoken/lpmanage](https://help.pandatool.org/createtoken/lpmanage)
* Solana增加与撤出流动性：[https://help.pandatool.org/sol/managepool](https://help.pandatool.org/sol/managepool)

**8.又有用户反馈，说我的项目没有锁池，我该怎么锁？**

答：锁池，就是将流动性凭证LP锁住，其目的在于无法撤池子。用户害怕你撤出流动性跑路，所以让你锁池。等到池子解锁，再撤出。不过这个概念在Solana上也叫烧池子，烧了之后就永远不能撤出了。不管是锁池还是烧池子，其目的都是为了防止项目方跑路。如果你需要锁池，那么可以使用PandaTool的锁工具来实现。（注意，锁池或者烧池不影响代币交易，池子依然存在.

* BSC/ETH锁池教程：https://help.pandatool.org/createtoken/createlock
* Solana烧池教程：[https://help.pandatool.org/sol/burn](https://help.pandatool.org/sol/burn)

**9.锁了池子后，又有用户反馈，说项目方持仓的代币数量太多了，能不能锁？**

答：同样可以，将代币锁住就是锁仓，本身就与锁池的概念一样。到了时间，代币才能取出。这样的目的，也是为了防止大户砸盘，是合理的。但是你只能锁自己钱包里面的代币，不能锁用户的代币。

* BSC/ETH锁仓教程：[https://help.pandatool.org/createtoken/createlock](https://help.pandatool.org/createtoken/createlock)

<figure><img src="https://academy.pandatool.org/wp-content/uploads/2025/10/2025102407460624-1000x440.png" alt=""><figcaption></figcaption></figure>

#### **四、其他可能遇到的问题**

**1.欧易钱包OKX提示：代币包含恶意代码是什么意思？**

答：出现这个提示的原因并不是代码中真的有恶意代码。因为像SOL代币合约SPL，用的都是统一标准的合约代码，不存在恶意代码的可能。那这个提示是什么意思呢？

简单来说，这是欧易的一次风险说明：它认为你这个代币有风险，就随便套用了一个提示说明，本质上就是不让你继续交易了。

那欧易OKX为什么认为这个代币有风险呢？主要是三个原因：

* **你没放弃权限**，例如增发/冻结权限，那就被判定为风险
* **你的资金池太小**，里面没有真实的USDT或者SOL，被OKX判定为假池子
* **你砸盘跑路，或者有砸盘的风险**。你持有的代币太多，存在砸盘跑路的可能性，所以风险太高

**2.在波场链发币为什么被识别为高风险？**

答：波场链的代币被识别为高风险诈骗币，主要原因是因为代币名称有问题。波场发币，不管是通过PandaTool创建代币，还是自己部署合约，代币名称都需要遵循以下原则：

* **不能与主流币名称相同或相似：**&#x4F8B;如名字里不能带USD、TRX、USDD等符号，这会被认为你是在做假币。
* **代币名称不能是网址/域名：**&#x4F8B;如你起一个名字是5644.com，这样就可能被认为是广告币，从而被屏蔽
* **代币名称不能是中文：**&#x4E0D;管是全称还是简称，都不能用中文起名字
* **代币名称不能是符号：**&#x4F8B;如emoji符号，就不能用作名称，否则会被识别为高风险

**3.PandaTool链接钱包为什么没有反应？**

答：假设您当前使用的设备是**手机**，那么您需要在手机的钱包App（内置浏览器.打开[发币网站](https://pandatool.org/)，然后切换到相应的链（如BSC，ETH等.，再连接钱包，就可以了。直接用手机自带的浏览器或者QQ浏览器这种，是无法连接钱包的。

假设您当前使用的设备是**电脑**，那么需要确定一下是否安装了钱包插件（谷歌浏览器扩展.。如果安装了插件依然不能连接钱包，可以适当关闭一些钱包插件。例如，同时有TP钱包插件、小狐狸钱包插件、OKX钱包插件的情况下，可以只保留一个OKX钱包插件，这样连接起来不容易混乱。

### **总结与展望**

至此，您已经完成了从“发币小白”到“准专家”的系统性学习。本指南涵盖了从概念解析、前期准备、实战发币到后期管理的全生命周期，希望能为您扫清迷雾，赋予您将想法落地的能力与信心。

区块链世界日新月异，新的链、工具和规则会不断涌现。**PandaTool团队将持续更新和维护本文档**，确保您所获取的信息始终处于前沿。

**获取最新信息，请务必收藏并关注我们的官方渠道：**

* **官方教程站**：[https://help.pandatool.org/](https://help.pandatool.org/)
* **官方交流群**：[https://t.me/pandatool](https://t.me/pandatool)

感谢您的阅读，祝您的发币之旅一切顺利！如果您有任何疑问，通过[Telegram](https://t.me/pandatool)与我们和广大开发者直接交流，我们始终为您提供支持。
