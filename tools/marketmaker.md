---
description: 针对代币在DEX进行批量交易与市值管理
icon: rotate
---

# DEX批量交易与市值管理教程

### **一、市值工具解读** <a href="#yi-shi-zhi-gong-ju-jie-du" id="yi-shi-zhi-gong-ju-jie-du"></a>

该工具是PandaTool开发、针对于以太坊兼容链的DEX市值管理工具，不仅支持了更多的链，工具速度、支持的资金池类型也有显著提升。

#### **1、功能概念** <a href="#id-1-gong-neng-gai-nian" id="id-1-gong-neng-gai-nian"></a>

用户可以导入多个钱包地址，针对某一代币进行批量交易。通过设定交易次数、交易价格等要素，来实现交易的停止与启动。其目的在于解放双手，快速实现代币的大量交易。

#### **2、支持类型** <a href="#id-2-zhi-chi-lei-xing" id="id-2-zhi-chi-lei-xing"></a>

该市值管理工具支持多条区块链、多个资金池类型，具体如下：

* **BNB Chain：**&#x50;ancakeSwap V2、PancakeSwap V3
* **Ethereum**：Uniswap V2、Uniswap V3
* **Avalanche：**&#x55;niswap V2、Uniswap V3
* **Polygon：**&#x55;niswap V2、Uniswap V3
* **Arbitrum、Optimsim、Base：**&#x55;niswap V2、Uniswap V3

### **二、市值工具使用教程** <a href="#er-shi-zhi-gong-ju-shi-yong-jiao-cheng" id="er-shi-zhi-gong-ju-shi-yong-jiao-cheng"></a>

我们打开市值工具的操作页面：[https://www.pandatool.org/zh-CN/market/uniswap](https://www.pandatool.org/zh-CN/market/uniswap) 然后根据以下教程进行操作

#### **1、查询资金池** <a href="#id-1-cha-xun-zi-jin-chi" id="id-1-cha-xun-zi-jin-chi"></a>

第一步，我们需要选择基础的信息，包括链、代币等：

<figure><img src="../.gitbook/assets/1链与池子配置.png" alt=""><figcaption></figcaption></figure>

* **选择链：**&#x9009;择您要交易的区块链，目标代币在哪条链，就选择哪条链
* **交易所：**&#x9009;择您创建的资金池类型，主要是V2和V3的区别
* **报价代币：**&#x5C31;是您的资金池代币，一般是BNB、ETH、USDT等，看下您的资金池交易对
* **代币地址：**&#x60A8;要交易的目标代币地址，直接填进来

确定好信息填写无误后，我们点击**查询**：

* 如果查询没问题，则页面右边会出现代币的价格，并提示您池子已经发现

<figure><img src="../.gitbook/assets/2代币价格正常.png" alt=""><figcaption></figcaption></figure>

* 如果查询有问题，会提示您未找到对应的交易池。这个时候，您需要核对选择的区块链或者交易所是否正确

<figure><img src="../.gitbook/assets/3未找到对应资金池.png" alt=""><figcaption></figcaption></figure>

#### **2、导入钱包** <a href="#id-2-dao-ru-qian-bao" id="id-2-dao-ru-qian-bao"></a>

查到资金池和价格后，我们点击右边的按钮导入钱包（私钥）

<figure><img src="../.gitbook/assets/4导入钱包 (1).png" alt=""><figcaption></figcaption></figure>

在弹出的页面输入钱包的私钥，一行一个，然后点击导入私钥。（一般导入几十个就可以了）

<figure><img src="../.gitbook/assets/5导入私钥 (1).png" alt=""><figcaption></figcaption></figure>

钱包导入之后，我们就能看到各个钱包地址了，然后点击**刷新余额**，确认一下钱包内的代币情况

<figure><img src="../.gitbook/assets/6刷新余额 (1).png" alt=""><figcaption></figcaption></figure>

余额刷新之后，我们进行下一步

#### **3、买入与卖出交易策略** <a href="#id-3-mai-ru-yu-mai-chu-jiao-yi-she-zhi" id="id-3-mai-ru-yu-mai-chu-jiao-yi-she-zhi"></a>

目前代币的交易方式有三种，分别是：**买入交易、卖出交易和刷量交易，**&#x540C;时会选择不同的操作类型。现在我们了解一下买入和卖出的交易设置

**金额类型（使用买入和卖出同理）**

<figure><img src="../.gitbook/assets/7金额类型 (1).png" alt=""><figcaption></figcaption></figure>

* **按照数量：**&#x8BBE;定每笔交易的买入数量，以报价代币计算（如USDT，BNB等）
* **按照比例：**&#x8BBE;定每笔交易钱包支出的余额比例
* **范围：**&#x8BBE;定交易数量或者比例的范围

**关于比例：**&#x8FD9;个比例是钱包余额的比例。如果您设置1%，钱包内1000U的话，那么第一笔交易就是10U。此时钱包内只有990U了，那么第二笔交易就是9.9U，以此类推

**停止类型（买入和卖出同理）**

<figure><img src="../.gitbook/assets/8停止条件.png" alt=""><figcaption></figcaption></figure>

* **按价格：**&#x5C31;是到了某个价格，停止交易
* **按次数：**&#x4EA4;易了多少次之后，就停止交易
* **间隔：**&#x6BCF;一笔交易的间隔时间，以秒为单位
* **线程数：**&#x540C;一秒发起多少笔交易，线程越大，交易频率越高（最大为6）

**设置案例**

例如我填写的代币交易设置是这样的：

<figure><img src="../.gitbook/assets/9交易策略.png" alt=""><figcaption></figcaption></figure>

这是一笔批量买入的交易，每次买入的金额是0.01USDT到0.1USDT之间。一共交易6次就停止，每次交易间隔时间为0\~3秒，不固定，线程数是1

设定完成后，我点击右边的开启交易按钮，即可开始交易

<figure><img src="../.gitbook/assets/10开始交易 (2).png" alt=""><figcaption></figcaption></figure>

从交易日志可以看到，一旦达到停止条件，会自动停止交易。

<figure><img src="../.gitbook/assets/11交易日志 (1).png" alt=""><figcaption></figcaption></figure>

#### **4、买卖交易设置** <a href="#id-4-mai-mai-jiao-yi-she-zhi" id="id-4-mai-mai-jiao-yi-she-zhi"></a>

不同于前面两种针对某个方向的交易，买卖交易指的是自动实现买和卖两种交易方式。

<figure><img src="../.gitbook/assets/12买卖刷量.png" alt=""><figcaption></figcaption></figure>

**金额类型（仅支持按数量交易）**

* **按数量：**&#x8F93;入您要交易的代币数量范围
* ~~**按比例：**&#x8BBE;定每笔交易钱包支出的余额比例~~

**买卖概率**

* **买单概率：**&#x7CFB;统发起一笔交易时，这笔交易是**买单**的概率有多大
* **卖单概率：**&#x7CFB;统发起一笔交易时，这笔交易是**卖单**的概率有多大
* 买单概率与卖单概率相加为100%

**数量设置**

* **买入：**&#x8BBE;置每笔买单的买入数量范围（如果数字一样，则为固定数量）
* **卖出：**&#x8BBE;置每笔卖单的卖出数量范围（如果数字一样，则为固定数量）

<img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FrWuBudOPZKINwYCXsrM8%252F13%25E4%25B9%25B0%25E5%258D%2596%25E6%2595%25B0%25E9%2587%258F%2520%25E8%258C%2583%25E5%259B%25B4.png%3Falt%3Dmedia%26token%3D7dc5ec25-1282-41ba-bbdb-856ec10d9164&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=bfef671a&#x26;sv=2" alt="" height="139" width="640">

**停止方式（设置交易次数）**

* **按次数：**&#x5F53;买卖笔数达到多少笔时停止交易
* ~~**按价格：**&#x8FBE;到多少价格时停止交易~~
* **间隔：**&#x6BCF;一笔交易的间隔时间，以秒为单位
* **线程数：**&#x540C;一秒发起多少笔交易，线程越大，交易频率越高（最大为6）

<img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FMnQnHyF2nTWxJiVIk2OR%252F14%25E4%25BA%25A4%25E6%2598%2593%25E5%2581%259C%25E6%25AD%25A2.png%3Falt%3Dmedia%26token%3D139ee1d0-173f-434d-8a28-96dae36237a6&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=8ae55946&#x26;sv=2" alt="" height="146" width="684">

设定完成后，我点击右边的开启交易按钮，即可**开始交易**

<figure><img src="../.gitbook/assets/13刷量交易.png" alt=""><figcaption></figcaption></figure>

### **三、疑问解答** <a href="#san-yi-wen-jie-da" id="san-yi-wen-jie-da"></a>

**1、代币地址没有错，为什么提示错误？**

* **答：**&#x5982;果确认代币地址没有错，那么可能是您选择的区块链错误，或者是交易所资金池类型错误

**2、为什么会交易失败？**

* **答：**&#x901A;常的原因是钱包内Gas不足或者代币余额不足导致的

**3、私钥会不会泄露？**

* **答：**&#x79C1;钥仅保存在您的电脑页面，不上传至服务器，至少PandaTool是看不到的

**4、最多可以导入多少钱包？**

* **答：**&#x7406;论上是没有上限的，但考虑到您的电脑CPU以及用户体验，几十个应该是比较合适的

**5、市值管理工具如何收费？**

* **答：**&#x5177;体每笔交易的费用如下
  * BSC 主网: 0.0005 BNB
  * Ethereum: 0.0001 ETH
  * Base: 0.0001 ETH
  * Arbitrum: 0.0001 ETH
  * Avalanche: 0.01 AVAX
  * Polygon: 0.1 POL
  * Optimism: 0.0001 ETH

如果您在市值管理工具的运行过程中，遇到了无法解决或者不清楚的地方，可以在PandaTool的官方交流群联系客服处理：[https://t.me/pandatool](https://t.me/pandatool)
