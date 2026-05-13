---
description: 使用PandaTool的批量交易机器人
icon: shuffle
---

# 代币批量交易/市值管理教程

## **一、市值工具解读**

该工具是PandaTool开发、针对于以太坊兼容链的市值管理工具升级版，不仅支持了更多的链，工具速度、支持的资金池类型也有显著提升。

### **1、功能概念**

用户可以导入多个钱包地址，针对某一代币进行批量交易。通过设定交易次数、交易价格等要素，来实现交易的停止与启动。其目的在于解放双手，快速实现代币的大量交易。

### **2、支持类型**

该市值管理工具支持多条区块链、多个资金池类型，具体如下：

* **BNB Chain：**&#x50;ancakeSwap V2、PancakeSwap V3
* **Ethereum**：Uniswap V2、Uniswap V3
* **Avalanche：**&#x55;niswap V2、Uniswap V3
* **Polygon：**&#x55;niswap V2、Uniswap V3
* **Arbitrum、Optimsim、Base：**&#x55;niswap V2、Uniswap V3

{% embed url="https://www.youtube.com/watch?v=jJ7xz8HlmIY" %}

## **二、市值工具使用教程**

我们打开市值工具的操作页面：[https://evmswap.pandatool.org/](https://evmswap.pandatool.org/)   然后根据以下教程进行操作

### **1、查询资金池**

第一步，我们需要选择基础的信息，包括链、代币等：

<figure><img src="../.gitbook/assets/1基础信息 (2).png" alt=""><figcaption></figcaption></figure>

* **选择链：**&#x9009;择您要交易的区块链，目标代币在哪条链，就选择哪条链
* **交易所：**&#x9009;择您创建的资金池类型，主要是V2和V3的区别
* **报价代币：**&#x5C31;是您的资金池代币，一般是BNB、ETH、USDT等，看下您的资金池交易对
* **代币地址：**&#x60A8;要交易的目标代币地址，直接填进来

确定好信息填写无误后，我们点击查询资金池：

* 如果查询没问题，则页面右边会出现代币i的价格，并提示您资金池正常

<figure><img src="../.gitbook/assets/3查询正常.png" alt=""><figcaption></figcaption></figure>

* 如果查询有问题，会提示您查询错误，您需要核对选择的区块链或者交易所是否正确

<figure><img src="../.gitbook/assets/2查询错误.png" alt=""><figcaption></figcaption></figure>

### **2、导入钱包**

查到资金池和价格后，我们点击右边的按钮导入钱包（私钥）

<figure><img src="../.gitbook/assets/4导入钱包.png" alt=""><figcaption></figcaption></figure>

在弹出的页面输入钱包的私钥，一行一个，然后点击导入私钥。（一般导入几十个就可以了）

<figure><img src="../.gitbook/assets/5导入私钥.png" alt=""><figcaption></figcaption></figure>

钱包导入之后，我们就能看到各个钱包地址了，然后点击**刷新余额**，确认一下钱包内的代币情况

<figure><img src="../.gitbook/assets/6刷新余额.png" alt=""><figcaption></figcaption></figure>

余额刷新之后，我们进行下一步

### **3、买入与卖出交易设置**

目前代币的交易方式有三种，分别是：**买入交易、卖出交易和刷量交易，**&#x540C;时会选择不同的操作类型。现在我们了解一下买入和卖出的交易设置

#### **金额类型（使用买入和卖出同理）**

<figure><img src="../.gitbook/assets/7金额类型.png" alt=""><figcaption></figcaption></figure>

* **按照数量：**&#x8BBE;定每笔交易的买入数量，以报价代币计算（如USDT，BNB等）
* **按照比例：**&#x8BBE;定每笔交易钱包支出的余额比例
* **范围：**&#x8BBE;定交易数量或者比例的范围

{% hint style="success" %}
**关于比例：**&#x8FD9;个比例是钱包余额的比例。如果您设置1%，钱包内1000U的话，那么第一笔交易就是10U。此时钱包内只有990U了，那么第二笔交易就是9.9U，以此类推
{% endhint %}

#### **停止类型（买入和卖出同理）**

<figure><img src="../.gitbook/assets/8停止类型.png" alt=""><figcaption></figcaption></figure>

* **按价格：**&#x5C31;是到了某个价格，停止交易
* **按次数：**&#x4EA4;易了多少次之后，就停止交易
* **间隔：**&#x6BCF;一笔交易的间隔时间，以秒为单位
* **线程数：**&#x540C;一秒发起多少笔交易，线程越大，交易频率越高（最大为6）

#### **设置案例**

例如我填写的代币交易设置是这样的：

<figure><img src="../.gitbook/assets/9交易设置.png" alt=""><figcaption></figcaption></figure>

这是一笔批量买入的交易，每次买入的金额是0.0001BNB到0.001BNB之间。一共交易6次就停止，没错交易间隔时间为0\~3秒，不固定，线程数是2.

<figure><img src="../.gitbook/assets/10开始交易.png" alt=""><figcaption></figcaption></figure>

设定完成后，我点击右边的开启交易按钮，即可开始交易

<figure><img src="../.gitbook/assets/11交易日志.png" alt=""><figcaption></figcaption></figure>

可以看到，如果钱包内gas不足，会直接跳过。一旦达到停止条件，会自动停止交易。

### **4、买卖交易设置**

不同于前面两种针对某个方向的交易，买卖交易指的是自动实现买和卖两种交易方式。

<figure><img src="../.gitbook/assets/12买卖设置.png" alt=""><figcaption></figcaption></figure>

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

<figure><img src="../.gitbook/assets/13买卖数量 范围.png" alt=""><figcaption></figcaption></figure>

**停止方式（设置交易次数）**

* **按次数：**&#x5F53;买卖笔数达到多少笔时停止交易
* ~~**按价格：**&#x8FBE;到多少价格时停止交易~~
* **间隔：**&#x6BCF;一笔交易的间隔时间，以秒为单位
* **线程数：**&#x540C;一秒发起多少笔交易，线程越大，交易频率越高（最大为6）

<figure><img src="../.gitbook/assets/14交易停止.png" alt=""><figcaption></figcaption></figure>

设定完成后，我点击右边的开启交易按钮，即可**开始交易**

<figure><img src="../.gitbook/assets/15开始交易.png" alt=""><figcaption></figcaption></figure>

## **三、疑问解答**

**1、代币地址没有错，为什么提示错误？**

* **答：**&#x5982;果确认代币地址没有错，那么可能是您选择的区块链错误，或者是交易所资金池类型错误

**2、为什么会交易失败？**

* **答：**&#x901A;常的原因是钱包内Gas不足或者代币余额不足导致的

**3、私钥会不会泄露？**

* **答：**&#x79C1;钥仅保存在您的电脑页面，不上传至服务器，至少PandaTool是看不到的

**4、最多可以导入多少钱包？**

* **答：**&#x7406;论上是没有上限的，但考虑到您的电脑CPU以及用户体验，几十个应该是比较合适的

**5、市值管理工具如何收费？**

* **答：**&#x60A8;可以在右上角查询我们的收费标准

<figure><img src="../.gitbook/assets/16收费标准 (1).png" alt=""><figcaption></figcaption></figure>

如果您在市值管理工具的运行过程中，遇到了无法解决或者不清楚的地方，可以在PandaTool的官方交流群联系客服处理：[https://t.me/pandatool](https://t.me/pandatool)
