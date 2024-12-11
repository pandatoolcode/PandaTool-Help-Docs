---
description: 公平做慈善、捐赠V神来炒作、打造新叙事
---

# 创建代币Mint捐赠预售教程

**什么是Mint捐赠预售？**

简单来说，就是通过Mint的方式预售，并将收到的BNB捐赠给名人钱包。j具体来说，项目方将一定数量的代币打入预售合约地址，开启预售后，用户将BNB转入预售合约地址，预售合约会自动按照设定好的比例，将一部分的代币或者BNB给到名人钱包，如V神钱包地址，方便后续的炒作。

和标准预售、加池预售不同，捐赠预售借助了名人营销的方式，主动的将V神等钱包地址加入到项目中来，给项目打造了新的叙事，便于后续的传播。

### 一、Mint捐赠预售功能说明 <a href="#id-1-gong-neng-jie-shi" id="id-1-gong-neng-jie-shi"></a>

* **捐赠预售：**&#x9884;售的同时将BNB或者代币给到名人钱包
* **无前端：**&#x4E0D;需要任何网页，纯合约支持，100%**去中心化**
* **转账即预售：**&#x7528;户将BNB转到`预售合约`，就能**自动**获得代币
* **自定义功能：**&#x9879;目方可以在预售开始后通过控制台**修改**预售价格和每份数量
* **无软顶/硬顶：**&#x6CA1;有软顶或者硬顶的概念，只有一个预售总数量（份数x每份数量）

### 二、注意事项提前说明 <a href="#er-zhu-yi-shi-xiang-ti-qian-shuo-ming" id="er-zhu-yi-shi-xiang-ti-qian-shuo-ming"></a>

* V神后期有砸盘的风险，注意防范
* 标准代币合约**不建议**开启预售，因为预售期间可能会有人加池
* 其他代币合约请不要开始交易（如有手动开盘功能的话）

### **三、捐赠预售创建教程** <a href="#san-mint-yu-shou-chuang-jian-jiao-cheng" id="san-mint-yu-shou-chuang-jian-jiao-cheng"></a>

**1、连接钱包（老手请忽略）**

首先，在小狐狸钱包里选择好币安链（BNB Smart Chain）

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FTPzIpsffzfaVswHf3TPQ%252F%25E5%25B8%2581%25E5%25AE%2589%25E4%25B8%25BB%25E7%25BD%2591.png%3Falt%3Dmedia%26token%3Dcf69fcf0-7085-43da-a2e9-414d3afdd8fd&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=d54bf4f&#x26;sv=2" alt=""><figcaption><p>小狐狸切换到币安链</p></figcaption></figure>

然后打开预售创建官网：[https://www.pandatool.org/#/presale/mintDonate](https://www.pandatool.org/#/presale/mintDonate)，点击右上角选择BSC链

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FXdGBxmzpnLvg1Gwd7rX9%252F%25E9%2580%2589%25E6%258B%25A9BSC.png%3Falt%3Dmedia%26token%3Dd43ec86c-ca1e-408b-b94f-9617a82cb8bc&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=93aa8c2b&#x26;sv=2" alt=""><figcaption></figcaption></figure>

然后选择右上角的连接钱包，会弹出小狐狸让你确定要连接的钱包地址，选择一个就行了

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FOfQAGYfGyFD3H0Bxlh1Q%252F%25E9%2580%2589%25E6%258B%25A9%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3D400d920c-7405-419f-9f3a-41e3e3fbfe04&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=3b1382d9&#x26;sv=2" alt=""><figcaption></figcaption></figure>

钱包连接完成后，能在右上角看到你的钱包地址和链状态，说明已经链接成功了

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fg3I4f6b2ZVOKuPRXnpx5%252F%25E9%2592%25B1%25E5%258C%2585%25E8%25BF%259E%25E6%258E%25A5%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3Df50147dc-25ea-4df0-8ae9-bd49ca0f85c8&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=c2c2a133&#x26;sv=2" alt=""><figcaption></figcaption></figure>

**2、填写预售参数**

钱包连接成功后，我们通过PandaTool可视化页面创建预售，还是那个页面[https://www.pandatool.org/#/presale/mintDonate](https://www.pandatool.org/#/presale/mintDonate) 打开，填写相应的预售参数：

