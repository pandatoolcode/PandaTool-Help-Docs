---
description: 通过区块链完成代币或者流动性的解锁
icon: unlock
---

# 代币与LP链上解锁教程

如果我们通过PandaTool将代币或者LP锁住了，没到解锁时间，PandaTool网站无法打开了（尽管这种情况发生的可能性几乎为0）。这种情况下，我们该如何完成代币或者LP的解锁呢？到了时间，我们该如何取回自己的代币？

今天这篇教程，就是教大家通过区块链浏览器来完成代币或者LP的解锁。

* PandaTool锁池工具：[https://pandatool.org/#/createLock?lang=zh-CN](https://pandatool.org/#/createLock?lang=zh-CN)
* PandaTool解锁工具：[https://pandatool.org/#/lockList?lang=zh-CN](https://pandatool.org/#/lockList?lang=zh-CN)

### **一、解锁操作指南**

首先，我们需要在区块链浏览器找到锁池合约（以BSC链为例）：[https://bscscan.com/address/0x407993575c91ce7643a4d4ccacc9a98c36ee1bbe#writeContract](https://bscscan.com/address/0x407993575c91ce7643a4d4ccacc9a98c36ee1bbe#writeContract)

<figure><img src="../.gitbook/assets/1web3 (2).png" alt=""><figcaption></figcaption></figure>

打开之后，点击那个**Connect to Web3，然后**连接上钱包

<figure><img src="../.gitbook/assets/2确定 (2).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/3链接钱包 (1).png" alt=""><figcaption></figcaption></figure>

需要注意的是，一定要用锁池/锁仓的那个钱包连接，不然没有意义。哪个钱包锁的，哪个钱包才有权限操作。

接下来，我们找到第7个选项：unlock，在里面需要输入一个数值lockid，指的就是锁ID

<figure><img src="../.gitbook/assets/4unlock (1).png" alt=""><figcaption></figcaption></figure>

这个ID是多少呢？我们不知道，需要去查。

怎么查？找到你当时锁池/锁仓的哈希，在区块链浏览器里搜索，然后点击那个logs

<figure><img src="../.gitbook/assets/5logs (1).png" alt=""><figcaption></figcaption></figure>

然后在最下面有两个数值，分别是ID和unlockDate，把这两个数值记下来：

<figure><img src="../.gitbook/assets/6数值 (2).png" alt=""><figcaption></figcaption></figure>

这个ID（1348849）就是刚才需要输入的，而这个unlockDate（1767110400）就是你的解锁日期。该数字需要通过时间戳来转换具体得日期时间，可以在这里转换：[https://tool.lu/timestamp/](https://tool.lu/timestamp/)

<figure><img src="../.gitbook/assets/7时间戳 (1).png" alt=""><figcaption></figcaption></figure>

可以看到，1767110400经过转换之后，就能获得一个时间是2025年12月31日。在这个时间，我们才能操作解锁。

假设你的锁时间已经过了，那么就会回到刚才的**unlok**操作页面，在输入框里输入**1348849**，然后点击**Write**，弹出钱包确认即可

<figure><img src="../.gitbook/assets/8unlock (2).png" alt=""><figcaption></figcaption></figure>

到这里，整个解锁流程就完成了。接下来，是一些可能涉及到的疑问，我也一并给大家解答一下

### **二、解锁疑问解答**

**1、为什么我点击write没有反应？**

* **答：**&#x53EA;有两个原因，要么是您没有连钱包，或者是链接的钱包不是当初锁的钱包。要么就是还没到解锁时间，所以操作不了。

**2、为什么我的时间戳转换的日期不对？**

* **答：**&#x65F6;间戳日期转换，分别有**秒**和**毫秒**两种格式。我们平台锁仓给的时间戳都是按照秒的格式转换，有些时间戳是毫秒，所以这个不要搞错了。如果不对，换一下就行

<figure><img src="../.gitbook/assets/9时间戳秒 (1).png" alt=""><figcaption></figcaption></figure>

**3、找不到当初锁的哈希怎么办？该如何获得时间戳以及LockID？**

* 答：如果操作时间太久，导致你找不到当时操作的锁池/锁仓哈希，以至于无法获得ID。那么还有其他办法。

我们需要在锁合约里Read Contact页面，找&#x5230;**`normalLocksForUser`**&#x51FD;数&#x548C;**`lpLocksForUser`**&#x51FD;数。进入页面：[https://bscscan.com/address/0x407993575c91ce7643a4d4ccacc9a98c36ee1bbe#readContract](https://bscscan.com/address/0x407993575c91ce7643a4d4ccacc9a98c36ee1bbe#readContract)

<figure><img src="../.gitbook/assets/10 foruser (2).png" alt=""><figcaption></figcaption></figure>

* **14  lpLocksForUser：**&#x5047;设你锁的是池子/LP，那么就在这里输入创建锁的钱包地址，点击**Query**，就能得到LockID，以及时间戳
* **17 normalLocksForUser：**&#x5047;设你锁的是代币，那么就在这里输入创建锁的钱包地址，点击**Query**，就能得到LockID，以及时间戳

<figure><img src="../.gitbook/assets/11查询 (1).png" alt=""><figcaption></figcaption></figure>

总的来说，针对代币和LP，分红要调用不同的合约函数去获得ID和时间戳，但流程都是一样的。

如果你针对这个锁还有什么问题，可以进入我们的官方Telegram，咨询志愿者：[https://t.me/pandatool](https://t.me/pandatool)
