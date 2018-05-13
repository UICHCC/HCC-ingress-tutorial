#Ingress-tutorial-UIC

<center>Under Construction</center>



## 剧情

* 广州蓝军开通了介绍游戏剧情的<a href ="https://telegram.me/ingress_story2016"> Telegram 频道</a> , 可以通过这个频道了解更多关于剧情的信息。
* 

## 下载并安装游戏

推荐使用 Android 设备进行游戏。iOS 系统对 APP 的诸多限制会带俩一些阻碍。

### Android

> 16 年 5月起，NIA 更新了作弊检测算法，导致部分国产安卓设备的定位算法（例如小米手机的智能省电模式）会与之冲突
> ，使用类似设备操作可能会导致误封，请与 NIA 联系
> 笔者曾经使用 ZUK Z2 因为室内打开游戏定位偏移导致永久封号，所以在此强烈建议，如果打开游戏后定位偏移，请不要 操作，或关掉游戏，等到达 GPS 正常的地方在进行游戏.

### 系统要求

* Android2.3 及更高版本
* 最新版本的 Google Play Service 
* 适合的可用空间
* GPS 模块

### iOS

请从 <a href="https://itunes.apple.com/us/app/ingress/id576505181?mt=8"> App Store </a> 直接下载

### 系统要求

- iOS 7.0 及更高版本
- 约 100M 可用空间
- 未越狱 [2]

在 Wi-Fi 版 iPad 和 iPod Touch 上，定位可能非常不准确（取决于所在区域），因此不建议使用这些设备。推荐使用 iPhone 或 Wi-Fi + Cellular 版本 iPad。

## 网络指南

可以通过各种途径进行「科学上网」，例如：Shadowsocks、V2ray，brook 等；鉴于 ingress 是一个对于网络实时性很高的游戏，所以，“水管”可以不大，但是延迟不能太高。

⚠️**ingress 无法通过 http代理服务器进行代理**

下面介绍一些笔者使用过的「科学上网」软件：

#### Android

##### Shadowsocks

目前较为稳定和使用较为广泛的是 [Shadowsocks](http://shadowsocks.org/)，该项目能稳定工作在多个平台，Android 上工作也非常稳定快速，同时，在 Android 5.0 及以上的设备上，其可以不需要 root 权限便工作在支持分应用代理的 VPN 模式下，Android 5.0 以下的设备也可以以中国路由的模式工作在 VPN 模式下。

Shadowsocks 项目本身仅提供协议和服务器 / 客户端实现，本身并未提供任何可以实现翻墙的服务器，此部分可以通过购买各类翻墙服务商提供的付费服务器或者自己租用 VPS 搭建服务器端实现。该部分不在本教程该范围内，请自行搜索或者咨询当地其它玩家。

##### ShadowsocksR

>  在ss作者被喝茶之后，github上出现了一个叫breakwa11(破娃)的帐号，声称ss容易被防火墙检测到，所以在混淆和协议方面做了改进，更加不容易被检测到，而且兼容ss，改进后的项目叫shadowsocks-R，简称ssr，然后ss用户和ssr用户自然分成了两个派别，互相撕逼，直到前阵子，破娃被人肉出来，无奈之下删除了ssr的代码，并且解散了所有相关群组。

 上述文字摘自：<a href="https://blog.csdn.net/Marvel__Dead/article/details/78495583">VPN 与 SS/SSR 的区别 </a>

#### iOS

（iOS 由于系统限制，Shadowsocks 并不能在非越狱的设备上稳定工作，因此，VPN 几乎是非越狱 iOS 设备的唯一选择，你可以选择自行搭建或者购买商业服务。）

#### 现在可以用 Surge 链接 Shadowsocks 翻墙实现 Ingress 游戏正常运行。

#### 规则中添加 DOMAIN-KEYWORD,google,Proxy,force-remote-dns 以及 DOMAIN-SUFFIX,appspot.com,Proxy,force-remote-dns。

[![Surge规则添加](https://hz-ingress.gitbooks.io/ingress-tutorial/content/before_game/images/image.jpeg)](https://hz-ingress.gitbooks.io/ingress-tutorial/content/before_game/images/image.jpeg)

#### 通过已翻墙的 Android 设备或者 Mobile Wi-Fi 设备上网

此方法在此不详述。

##### Shadowrocket

Shadowrocket，我们俗称的小火箭，因为其图标是一个小火箭的LOGO，所以大家爱称之为小火箭。大家到App Store下载的时候别认错了，App Store好几款挂羊头卖狗肉的冒充货。 Shadowrocket是一款基于规则的网络调试工具，具有性能高和稳定好、使用流畅，功能多样的特点，只占用最少的系统资源，全盘接管所有的连接，根据规则来进行处理，让你无忧无虑。独有的场景模式，方便根据不同需求自动切换配置及节点。

目前，此软件以由于各种原因退出国区，请使用美区/港区/日区 的 Apple ID 进行下载

<a href"https://itunes.apple.com/us/app/shadowrocket/id932747118?mt=8">App Store</a> 链接

