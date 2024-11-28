---
description: 干净合约、方便上手、无税无功能、Ave检测全绿
---

# 🔥 标准代币

标准代币开发视频教程：

{% embed url="https://www.youtube.com/watch?v=zUAvX5MfMO8" %}

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

代币创建完成之后，只能转账，还不能交易。要想使代币可以交易，需要前往PancakeSwap创建一个流动性资金池才可以。

首先，我们打开薄饼的官网：[https://pancakeswap.finance/?chain=bsc](https://pancakeswap.finance/?chain=bsc) ,点击右上角连接钱包

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FU83ogc8KndoziTUSyDIG%252F%25E9%2593%25BE%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3Db960910a-52d6-474c-b268-eb47c5308029&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=c77ce06&#x26;sv=1" alt=""><figcaption></figcaption></figure>

此时会跳出提示，让你选择钱包类似，电脑默认都是选择Metamask，之后小狐狸会提示让你确认

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FLHeO8bTUQjIQVtWDYwaV%252Fmetamask%25E9%2593%25BE%25E6%258E%25A5.png%3Falt%3Dmedia%26token%3D10584b0c-7090-4dbc-ac7c-1eecb0270cb7&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=2a0e31ec&#x26;sv=1" alt=""><figcaption></figcaption></figure>

连接成功之后，右上角会出现你的钱包地址

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fn2u8qz8GoHeurkeN1XjW%252F%25E9%2593%25BE%25E6%258E%25A5%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3D8ab9f46e-7edf-472d-9111-4718bee17ef6&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=2e15fee1&#x26;sv=1" alt=""><figcaption></figcaption></figure>

钱包链接成功之后，在上方菜单栏找到“赚取”，然后选择“农场/流动性”

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FAT4fMITXZi90oZ0E4qRG%252F%25E5%258D%259A%25E9%25A5%25BC1.png%3Falt%3Dmedia%26token%3D9113c468-3457-45d0-9c63-34d703edbddf&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=7a895c44&#x26;sv=1" alt=""><figcaption></figcaption></figure>

在打开的新页面里，选择“我的持仓”（或者直接进入链接：[https://pancakeswap.finance/liquidity/positions](https://pancakeswap.finance/liquidity/positions)）

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FmQoumcRANrPYjjAAuy76%252F%25E5%258D%259A%25E9%25A5%25BC2.png%3Falt%3Dmedia%26token%3Dae8a4f80-6dcc-4854-ac15-718ec06215c9&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=e61b7b3f&#x26;sv=1" alt=""><figcaption></figcaption></figure>

之后在右边可以看到添加流动性的按钮

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FnPQayB26XX1inNvO0Gkf%252F%25E5%258D%259A%25E9%25A5%25BC3.png%3Falt%3Dmedia%26token%3D566c38bd-38b5-45d8-bb04-6b1c59691003&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=4c025e44&#x26;sv=1" alt=""><figcaption></figcaption></figure>

然后会看到两个代币对提示框，在两个选择您想要添加流动性的交易对中的两个代币

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fz2NvxvJBR9ut3hYqRWnc%252F%25E9%2580%2589%25E6%258B%25A9%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3Dee2f1136-d933-496c-859d-9185dcceb0f6&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=a0594298&#x26;sv=1" alt=""><figcaption></figcaption></figure>

一般来说，左边选择BNB或者USDT，右边搜索选择你自己的代币

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fq0Fjd2veYJgqs7qoHzy4%252F%25E5%2590%2588%25E7%25BA%25A6%25E5%259C%25B0%25E5%259D%2580.png%3Falt%3Dmedia%26token%3D5ea4f867-726f-4d51-89c7-e9532b3eed90&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=f6f7743b&#x26;sv=1" alt=""><figcaption></figcaption></figure>

例如我选择的交易对：USDT-Panda。选择好交易对之后，记得选&#x62E9;**“添加V2流动性”**，这一步非常重要请谨记。V3流动性只适合标准币，除此之外，必须都加V2的流动性

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FWL77qCvowfc5G0jZcFHg%252FV2%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3Dccc64b5e-90e1-4ee7-8856-8be67165cdef&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=d5c00560&#x26;sv=1" alt=""><figcaption></figcaption></figure>

之后，我们根据自己的需求，填写注入流动性资金池的代币数量。两个代币数量的比例，决定了代币的初始价格。例如，我添加1000USDT和1000个Panda，说明代币的上线价格是1U

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FV8GsgDx4U6UE8VxM9fTr%252F%25E6%25B7%25BB%25E5%258A%25A0%25E4%25BB%25A3%25E5%25B8%2581%25E6%2595%25B0%25E9%2587%258F.png%3Falt%3Dmedia%26token%3D04699c7d-6428-41dc-9ee4-d50094602a08&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=bd6ec72d&#x26;sv=1" alt=""><figcaption></figcaption></figure>

然后依次授权USDT和你自己发行的代币

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F01Oz6jKTfHkq7BOxWlIV%252F%25E7%25A1%25AE%25E8%25AE%25A4%25E6%258E%2588%25E6%259D%2583.png%3Falt%3Dmedia%26token%3D90b360ce-c3fb-478d-8c66-abe1d1c383ff&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=54a9d562&#x26;sv=1" alt=""><figcaption></figcaption></figure>

授权成功后点击“添加”，metamask钱包进行确认即可

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FnWD0gT5JIQQIzDKSxYNJ%252F%25E6%25B7%25BB%25E5%258A%25A0.png%3Falt%3Dmedia%26token%3Da6d287df-de4a-483e-8b35-1fb082343db7&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=1c315c69&#x26;sv=1" alt=""><figcaption></figcaption></figure>

添加完成后，我们回到上一页，就能看到自己的池子信息了

<figure><img src="https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FccA68CX5iVZH4KAJLhjJ%252F%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7%25E6%2598%25BE%25E7%25A4%25BA.png%3Falt%3Dmedia%26token%3De760965f-7e7e-4f52-ab57-621f5a6a165a&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=d79852ca&#x26;sv=1" alt=""><figcaption></figcaption></figure>

## 注意事项

* 代币创建完成后，默认是开源的，无需手动开源。
* 如果您要在测试网添加USDT交易对，请使用PandaTool官方发布的测试USDT做资金池，合约地址：0x66e972502a34a625828c544a1914e8d8cc2a9de5
