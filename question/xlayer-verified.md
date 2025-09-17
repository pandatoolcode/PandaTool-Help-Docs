---
description: 在OKLink浏览器为X Layer代币开源
icon: lock-open
---

# X Layer代币怎么开源验证？

很多人在PandaTool创建了代币后不知道怎么开源，今天这个教程，就是教大家为X Layer（OK链）代币进行开源验证。

### **什么是开源？**

所谓开源，就是将代币合约代码完完整整的展示出来，让任何人都可以通过区块链浏览器看到你的代币代码，这样代码里有没有后门就一目了然了，开源的目的也是为了让用户放心，

### **如何开源？**

不同区块链的代币开源逻辑不一样，例如以太坊、BSC等区块链的代币，一般都是自动在浏览器里开源的。但是X Layer的代币，则需要通过OKLink浏览器手动开源。

接下来，将为大家详细展示在PandaTool发行的代币该如何开源验证。

#### **1、打开浏览器**

首先，我们需要先进入浏览器的开源验证页面：[https://www.oklink.com/zh-hans/x-layer/verify-contract-preliminary](https://www.oklink.com/zh-hans/x-layer/verify-contract-preliminary)

<figure><img src="../.gitbook/assets/1 (6).png" alt=""><figcaption></figcaption></figure>

#### **2、选择基础参数**

之后，我们在相对应的界面填写基础参数

* **合约地址：**&#x4EE3;币的合约地址
* **编译器类型：**&#x53;olidity(SingleFile)
* **编译器版本：**&#x76;0.8.18+commit.87f61d96

<figure><img src="../.gitbook/assets/2 (8).png" alt=""><figcaption></figcaption></figure>

选择好之后，点击下一步

#### **3、输入合约源码并配置高级参数**

接下来，我们需要详细的进行参数配置，同时填入合约源码（大家看好自己的机制，是什么机制的代币，就下载哪个合约）

{% file src="../.gitbook/assets/标准代币-合约源码.txt" %}

{% file src="../.gitbook/assets/LP分红-合约源码.txt" %}

{% file src="../.gitbook/assets/LP分红+推荐奖励-合约源码.txt" %}

{% file src="../.gitbook/assets/黑洞分红-合约源码.txt" %}

{% file src="../.gitbook/assets/314协议-合约源码.txt" %}

{% file src="../.gitbook/assets/持币复利+推荐奖励-合约源码.txt" %}

{% file src="../.gitbook/assets/Mint+持币暴力分红-合约源码.txt" %}

{% file src="../.gitbook/assets/Mint+底池燃烧-合约源码.txt" %}

{% file src="../.gitbook/assets/LP挖矿+推荐奖励-合约源码.txt" %}

* **是否优化：**&#x662F;
* **优化：**&#x32;00（注意：**`Mint+暴力分红`**&#x548C;**`黑洞分红`**，这两个合约的优化数字是**10**，其余200）
* **是否基于 IR：**&#x5426;
* **合约源码：**&#x4E0B;载上面的文件，并复制填入
* **ABI 数据：**&#x4E0D;用管
* **引用的合约地址 (选填)：**&#x4E0D;用管
* **开源许可类型：**&#x4D;IT License (MIT)
* **虚拟机版本：**&#x64;efault（默认的）

<figure><img src="../.gitbook/assets/4-44 (1).png" alt=""><figcaption></figcaption></figure>

#### **4、提交并等待**

确认好所有的信息后，点击提交

<figure><img src="../.gitbook/assets/5 (3).png" alt=""><figcaption></figcaption></figure>

等待几秒钟，就会出现验证成功的提示

<figure><img src="../.gitbook/assets/7 (4).png" alt=""><figcaption></figcaption></figure>

#### **5、合约已验证开源**

此时，我们在OKLink浏览器搜索这个代币，就能看到合约已经开源验证的提示

<figure><img src="../.gitbook/assets/8 (3).png" alt=""><figcaption></figcaption></figure>

### 开源问答

**1、为什么会开源失败？**

* **答：**&#x56DE;到上一步看一下选择的参数是不是错了，仔细核对下。以及代码是否是正确的。

**2、不是PandaTool发的币可以开源吗？**

* **答：**&#x6309;照这个流程可以开源，但是源码需要是你自己的源码，参数也会不同。当前这个文档上传的源码，是我们平台的。

**3、为什么验证成功后，OKX钱包还是提示未开源？**

* **答：**&#x53EF;能是检测延迟，等一段时间看看

**4、任何人都可以开源吗？还是必须权限钱包才可以？**

* **答：**&#x6309;照上述教程，任何人都能开源，无需权限地址操作

**5、代币开源需要额外收费吗？**

* **答：**&#x5F00;源是完全免费的，无需任何费用

如果您是在PandaTool创建的代币，但是无法开源，或者遇到问题，可以在我们群里咨询志愿者：[https://t.me/pandatool](https://t.me/pandatool)

