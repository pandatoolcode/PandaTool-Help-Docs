---
description: 干净合约、方便上手、无税无功能、Ave检测全绿
icon: square-1
---

# 标准代币

BSC链代币创建教程视频

{% embed url="https://www.youtube.com/watch?v=ma3moINidRg" %}

## 1、功能解释

标准代币指的是**没有任何功能**、机制的代币合约，代币创建之后默认会丢弃权限，所以也没有任何权限，是一个纯粹的、干净的、标准的合约。

根据以下步骤，您可以在可支持的任意一条链上，创建一个标准合约代币。以BSC为例。

* 注意：没有安装小狐狸钱包的不能发币，请先安装小狐狸钱包插件，教程：[https://help.pandatool.org/practical-information/metamask](https://help.pandatool.org/practical-information/metamask)

## 2、连接钱包

使用浏览器或者钱包打开网址：[https://pandatool.org/#/coinrelease/stardand](https://pandatool.org/#/coinrelease/stardand)，点击右上角，将小狐狸钱包切换到币安主网（BSC）

<figure><img src="../.gitbook/assets/微信截图_20240117222904.png" alt=""><figcaption></figcaption></figure>

## 3、填写代币参数

在打开的页面，依次填写代币信息。假设我们创建一个代币叫——“PandaTool”，应该进行如下填写：

* **代币名称：**&#x50;andaTool（代币全称）
* **代币符号：**&#x50;anda（代币简称）
* **发行量：**&#x31;0000（代币数量）
* **精度：**&#x31;8（小数点后的位数）

<figure><img src="../.gitbook/assets/标准代币.png" alt=""><figcaption><p>标准代币</p></figcaption></figure>

## 4、创建合约

确认填写的参数无误后，点击“创建合约”。在打开的页面，将源代码和构造参数复制下来，以防万一：

<figure><img src="../.gitbook/assets/开源参数.png" alt=""><figcaption><p>开源参数复制</p></figcaption></figure>

复制之后，再次点击“创建合约”。此时小狐狸钱包会要求你支gas费，点击确认，等待几十秒，合约就创建完成了。

此时，我们点击`控制台`，就能看到自己创建的合约了，代币也已经发送到创建者的钱包地址里。

<figure><img src="../.gitbook/assets/进入控制台.png" alt=""><figcaption><p>进入控制台</p></figcaption></figure>

## 5、添加流动性

代币创建完成之后，只能转账，还不能交易。要想使代币可以交易，需要创建一个流动性资金池才可以。

### **1）进入PandaTool并连接钱包**

我们进入到PandaTool创建资金池工具的网页：[https://www.pandatool.org/#/createliquidity?lang=zh-CN](https://www.pandatool.org/#/createliquidity?lang=zh-CN) 然后在右上角点击连接钱包

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FPbbxvTJpKvA77TCQ9Tqg%252F1.%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3D8dd6bd7f-1a0a-48c6-9946-129526d05c60&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=86bf2953&#x26;sv=2" alt=""><figcaption></figcaption></figure>

此时会跳出Metamask或者OKX Web3钱包，点击确认，即可完成连接。钱包连接成功后，会在右上角看到你的钱包地址。

如果你希望在BSC链创建资金池，就将区块链切换到BSC。如果是希望在以太坊上创建资金池，就将区块链切换到ETH即可

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F1w5qQjQSljaqv4Dbi0Tk%252F2.%25E8%25BF%259E%25E6%258E%25A5%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3Daa876443-0773-451e-90d8-e8643228e373&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=26ac03ef&#x26;sv=2" alt=""><figcaption></figcaption></figure>

### **2）选择代币** <a href="#id-2-xuan-ze-dai-bi" id="id-2-xuan-ze-dai-bi"></a>

连接钱包后，我们需要选择加池类型和代币

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FZT8rDfyfi6Jtfuj2gjiu%252F3%25E9%2580%2589%25E6%258B%25A9%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3Dcb02c7a2-e16f-4009-b50e-0f9111029d9e&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=763a79b3&#x26;sv=2" alt=""><figcaption></figcaption></figure>

* **加池类型：**&#x9ED8;认用V2，稳定池加V3
* **底池代币：**&#x4EA4;易对价值代币，如USDT、BNB等
* **代币地址：**&#x60A8;创建的代币合约地址

填写好之后，点&#x51FB;**`查询代币`** ，正常来说会提示你：**代币正常，请填写加池数量**

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FOGrX5fvZTzORDK0dCJoc%252F4%25E5%258A%25A0%25E6%25B1%25A0%25E6%2595%25B0%25E9%2587%258F.png%3Falt%3Dmedia%26token%3D5b86d10f-a099-423c-9c5a-3b10cbd5db74&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=cc26fa49&#x26;sv=2" alt=""><figcaption></figcaption></figure>

### **3）填写加池数量** <a href="#id-3-tian-xie-jia-chi-shu-liang" id="id-3-tian-xie-jia-chi-shu-liang"></a>

确定好两种代币后，接下来就是填写代币数量了（加池数量不能超过自己钱包里的数量）

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FhSAXnwjXJmMKZk7CpF4M%252F5%25E5%258A%25A0%25E6%25B1%25A0%25E6%2595%25B0%25E9%2587%258F2.png%3Falt%3Dmedia%26token%3D1c72c1bb-7067-430b-962d-e29629f038be&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=dd7453e&#x26;sv=2" alt=""><figcaption></figcaption></figure>

* **Panda：**&#x6211;创建的代币，填写10000枚，表示将10000个Panda代币放入资金池中
* **USDT：**&#x6211;选择的价值嗲比，填写10000，表示将10000个USDT放入资金池中

**预估价格：**&#x50;anda代币的初始价格是1USDT（用10000除以10000得到价格是1）。如果Panda放1000个，USDT放10000个，那么预估初始价格就是10U，以此类推

### **4）代币授权** <a href="#id-4-dai-bi-shou-quan" id="id-4-dai-bi-shou-quan"></a>

当我们确定好加池的代币和数量之后，就需要钱包授权了。也就是说，你要将代币授权给路由合约，然后路由合约会帮助你完成加池操作。

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FGeMSQ6p44y64PFQG5fqt%252F6%25E4%25BB%25A3%25E5%25B8%2581%25E6%258E%2588%25E6%259D%2583.png%3Falt%3Dmedia%26token%3Db5b2fa56-45ea-4bc1-9248-9e70c1e52ed6&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=69773d02&#x26;sv=2" alt=""><figcaption></figcaption></figure>

我们需要分别对两种代币进行授权（如果是BNB或者ETH，则无需授权），此时会跳出钱包进行确认

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fl3i0OVoKNWffqozv82tY%252F7%25E6%258E%2588%25E6%259D%2583%25E6%258F%2590%25E7%25A4%25BA.png%3Falt%3Dmedia%26token%3D5ec2687f-4bb1-44a1-9871-ae8c80242a8c&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=a2195cc2&#x26;sv=2" alt=""><figcaption></figcaption></figure>

当两种代币都授权成功后，会看到以下提示

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FLKkMqMVD4wCBNKM9nM1w%252F8%25E5%25B7%25B2%25E6%258E%2588%25E6%259D%2583.png%3Falt%3Dmedia%26token%3D8d3da2d0-d36c-4996-8dbd-22f886141257&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=e7da7db8&#x26;sv=2" alt=""><figcaption></figcaption></figure>

### **5）创建资金池** <a href="#id-5-chuang-jian-zi-jin-chi" id="id-5-chuang-jian-zi-jin-chi"></a>

代币授权完成后，就是创建资金池了。点击“立即加池”按钮，跳出钱包进行确认

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FE0nEZBS7LZZrNXaJY62g%252F10%25E5%258A%25A0%25E6%25B1%25A0%25E6%258F%2590%25E7%25A4%25BA.png%3Falt%3Dmedia%26token%3Dcffe5b72-d29f-4e7b-acd0-311e2794d90b\&width=768\&dpr=4\&quality=100\&sign=997908b5\&sv=2)

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FguRrJDgzgmpDwW7YPUAc%252F9%25E7%25AB%258B%25E5%258D%25B3%25E5%258A%25A0%25E6%25B1%25A0.png%3Falt%3Dmedia%26token%3D20531d92-8579-4058-bee5-c1d71ed4fd9b&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=cc14d5c9&#x26;sv=2" alt=""><figcaption></figcaption></figure>

钱包确认后等待几秒钟，即可完成创建资金池的操作

## 注意事项

* 代币创建完成后，默认是开源的，无需手动开源。
* 如果您要在测试网添加USDT交易对，请使用PandaTool官方发布的测试USDT做资金池，合约地址：0x66e972502a34a625828c544a1914e8d8cc2a9de5

如果您有任何关于发币的问题，均可以在Telegram群里咨询我们的志愿者：[https://t.me/pandatool](https://t.me/pandatool)
