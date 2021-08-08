# Windows 客户端使用 Shadowsocks 教程
 
Shadowsocks 是比VPN更科学的一种网络代理，使您可以访问到世界任何角落的互联网，所以越来越多的人开始使用。因此本文整理了Windows 客户端使用 Shadowsocks 的下载方法与使用教程，希望能给大家提供帮助。

## 下载方法
Windows客户端就是shadowsocks-windows，下载地址如下：

|Windows客户端|下载|
|----|----|
|最新版 Shadowsocks-4.4.0.0|[点击下载](https://github.com/shadowsocks/shadowsocks-windows/releases/download/4.4.0.0/Shadowsocks-4.4.0.185.zip)|
|XP系统 Shadowsocks-3.2|[点击下载(https://github.com/shadowsocks/shadowsocks-windows/releases/download/3.2/Shadowsocks-3.2.zip)]|
|更多版本|[点击下载](https://github.com/shadowsocks/shadowsocks-windows/releases)|

注意：安装过程中，若提示.NET framework过低，则需要下载.NET framework软件（.NET Framework 4.6.2 和 Microsoft Visual C++ 2015 Redistributable (x86)），[点击下载](https://www.microsoft.com/zh-CN/download/details.aspx?id=53344)，安装成功后，重新打开运行即可。

## 使用教程

下载完成后解压文件，打开EXE文件安装后，如下图所示，右键单击左下角任务栏的Shadowsocks【小飞机图标】进行配置：

![下载.png](https://i.loli.net/2021/08/08/HTi3fPgr76mLMC9.png)

在 【服务器】 菜单添加服务器节点。【服务器节点获取】详见：SS/ShadowsocksR 服务器节点 点击获取

接着如图所示，选择 "启用系统代理"来启用系统代理。注：请禁用浏览器里的代理插件，或把它们设置为使用系统代理

![启动代理系统.png](https://i.loli.net/2021/08/08/uqpUG3gFwjdr7TA.png)

最后可以打开 www.google.com 进行测试，一般来说就可以自由上网了。（若游览器无法打开google.com等网页，可能是你的游览器有插件或者设置了代理，可以尝试更换游览器测试一下）

## 更多说明

1、关于系统代理模式的区别：
1. 全局模式：你可能会遇到一些网站打不开，仍然无法访问，这个你可以试试选择【系统代理模式-全局模式】，这样使全部流量经过节点服务器。
2. PAC模式【推荐】：选择PAC模式，PAC文件网址列表走节点服务器，国内网址则走你自己使用的网络流量。

关于PAC更新，你可以直接从 GFWList （由第三方维护）更新 PAC 文件，或者你可以手动编辑本地pac文件。需要更新PAC：依次操作：PAC ->从GFW List更新PAC （等待更新完毕后）->使用本地PAC->启动系统代理。

2、服务器自动切换

负载均衡：随机选择服务器

高可用：根据延迟和丢包率自动选择服务器

累计丢包率：通过定时 ping 来测速和选择。如果要使用本功能，请打开菜单里的统计可用性。

也可以实现 IStrategy 接口来自定义切换规则，然后给我们发一个 pull request。

3、UDP

对于 UDP，请使用 SocksCap 或 ProxyCap 强制你想使用的程序走代理。

4、多实例

如果想使用其它工具如 SwitchyOmega 管理多个服务器，可以启动多个 Shadowsocks。 为了避免配置产生冲突，把 Shadowsocks 复制到一个新目录里，并给它设置一个新的本地端口。

5、插件

若想通过插件来连接服务器，请到编辑服务器界面填入插件程序（相对路径或绝对路径）

注意： 在启用插件后，正向代理会被停用。

### [<< 返回首页](README.md)


