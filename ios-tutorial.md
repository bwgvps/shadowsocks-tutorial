# iOS 苹果手机客户端使用 Shadowsocks 教程

在iOS苹果上使用Shadowsocks需要下载特定的客户端，常用的包括Shadowrocket和Potatso，为了大家的下载与使用更加便利，本文就此做出了详细的整理。

## 下载方法

由于一些原因，App Store中国大陆地区已下架所有VPN应用，包括Shadowrocket/Potatso，一般来说，国内用户想要下载Shadowrocket/Potatso，有以下两种解决方案。

解决方案

1.申请国外地区AppleID(推荐)或者某宝购买，使用他人的AppleID 一定不要开iCloud同步。

2.手机越狱(不推荐)

## 使用方法

### Shadowrocket （小火箭）使用教程

点击上方链接，下载手机客户端。

完成后进行获取一个可用的 Shadowsocks 账户（需要包括以下信息：服务器地址、端口号、加密方式、密码）。详见：SS/ShadowsocksR 服务器节点 点击获取

接着开始配置 Shadowsocks :

第一步添加 Shadowsocks 账户

Shadowrocket 是一款专门为 Shadowsocks 设计的 APP，所以添加起来也是极其方便。如下图，点击左上角的方框即可扫描 Shadowsocks 账户服务器节点的二维码，免去输入的麻烦。

![Shadowrocket添加账户.png](https://i.loli.net/2021/08/08/FgMwnVfkW16Euhx.png)

第一次连接时会弹出一个添加代理的提示框，选中“Allow”点击允许。如果你有多个节点，连接后是使用前面有圆点的节点，点击节点即选中作为默认，选中的节点使用中无法删除。

![Shadowrocket第一次连接.png](https://i.loli.net/2021/08/08/PskyfdOnzweSrY3.png)

或者你也可以点击右上角的加号进行手动输入，主要包括服务器地址、端口、密码等信息：

![Shadowrocket手动输入.png](https://i.loli.net/2021/08/08/SOcsFMtwjlQKe6r.png)

第二步设置规则：

一般来说，全局路由选择默认配置即可。如果要实现部分网站国内走直连，国外走代理的话，就需要用到规则。

如下图，点击 Settings，然后在点击 Config 你就可以看到以下界面：

![Shadowrocket设置规则.png](https://i.loli.net/2021/08/08/cSmsdot4PQCZXK8.png)

然后在上图页面中点击“ +” 通过添加链接，再点击 Use Config 来下载规则文件。接着点击感叹号，然后在点击 Add Rule，点击 Type，就可以看到多种过滤方式进行设置了。

第三步节点订阅设置：

如下图，打开Shadowrocket，点击右上角加号“ + ”，然后在添加节点页面，将类型改为第三个 Subscribe，复制订阅地址粘贴到URL中，然后点击右上角完成即可。

![Shadowrocket添加节点.jpg](https://i.loli.net/2021/08/08/JBqpHhzIfsneaL3.jpg)

然后在Shadowrocket设置–服务器订阅中打开【打开时更新】选项：

![Shadowrocket实时更新.png](https://i.loli.net/2021/08/08/YhmEc4x9JqTCbVZ.png)

最后回到首页，打开连接开关，就能享受科学上网啦！

### Potatso Lite 代理工具  使用教程

从 App Store 安装后打开 Potatso Lite。点击 “立即使用” 然后点击 “现在添加“：

![PotatsoLit现在添加.png](https://i.loli.net/2021/08/08/xKA2ZGnoyrE38WJ.png)

第一步进行配置，可以选择通过扫码的方式添加好节点，也可以手动配置。

如果进行手动配置，操作如下图，首先点击 “添加” 然后填写代理。接着选择 “Shadowsocks“ 开始填写服务器、端口、加密、密码。最后填写 “备注” 为可选项 >，完成后点击右上角的 “✔”， 设置完成。：

![PotatsoLite手动配置.png](https://i.loli.net/2021/08/08/eIFOxynzBTi8oWl.png)

第二步开始代理，点击 “开始”选项， 然后选择 “Allow” i开启 “智能路由”。当看到左上角出现 VPN 字样时，代表连接成功：

![PotatsoLite开始代理.png](https://i.loli.net/2021/08/08/oRUTaOedYIlw8ZH.png)

以上操作完成后，就可以使用Potatso Lite 代理工具去上网了。

### [<< 返回首页](README.md)
