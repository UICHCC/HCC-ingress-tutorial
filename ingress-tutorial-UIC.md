# Ingress-tutorial-UIC

<center>Under Construction</center>



## 剧情

* 广州蓝军开通了介绍游戏剧情的<a href ="https://telegram.me/ingress_story2016"> Telegram 频道</a> , 可以通过这个频道了解更多关于剧情的信息。
* 台湾绿军发布的 [INGRESS 中文劇情時間線](http://www.ingress.game.tw/2016/03/ingress.html)，是目前中文剧情比较全面的文章，推荐阅读。

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

<a href="https://itunes.apple.com/us/app/shadowrocket/id932747118?mt=8">App Store</a> 链接

## 教程

### 基础描述

该游戏的主要目标是阻止未知的塑造者 (Shaper) 的军队占领人类世界，或者您也可以根据自己的想法，选择与塑造者结盟，帮助他们完成对人类的 “启蒙”。这要通过与 Resistance 或 Enlightened 中的一个阵营结盟和在地理区域上创立 Control Filed 实现。游戏的进度由各个阵营分别控制的 Mind Units 数量来衡量（可以参见 [Intel Map](https://ingress.com/intel)）。

------

您可以占领 Portal 并将其 Link 起来形成 Field，以建立 XM Control Field。越强大的 Portal 其连接距离越长（最远可达数百公里）。据点的连接范围由其上部署的 Resonator 的能量决定。必须使用 Portal Key 才能形成 Link。

------

当三个 Portal 两两连接形成一个三角形时，一个 Control Field 就在这个区域上方建成了。在 Scanner 上，Control Field 会显示为该区域上方一个模糊的蓝色或绿色领域。占领的 Mind Units 的数量与所覆盖区域的人口密度有关。城市相较于农村地区能产生更多的 Mind Units。

您的终极目标是与您所在阵营里的其他玩家合作，共同维护全世界的安全或解放全世界。

#### Scanner

Scanner 指安装 Ingress 的任何设备（例如手机、平板或其他设备）。Scanner 扫描到附近的一切 portal 及道具都会展示在主界面上。

Scanner 是特工与 Ingress 交互的设备。借助 Scanner，特工可以操作 portal 及使用道具。初次之外，Scanner 还提供了 COMM 以便特工之间交流。

> 简单讲，Scanner 就是特工手机中的 Ingress APP。

#### 术语表

*本文介绍游戏中常用的术语。括号内为玩家间的俗称。*

| 术语（俗称）           | 注解                                                         |
| ---------------------- | ------------------------------------------------------------ |
| AP（经验值）           | 在您完成任务（例如占领据点、创建连接和建立控制场）时赢得的分数。 |
| 冷却期                 | 您为获取物品而再次入侵攻击过的同一个据点前必须等待的一段时间。 |
| 控制场                 | 连接三个据点即可形成一个控制场。建立控制场可以增加您所在阵营的思想单位的分数，且增加的分数取决于该控制场所包含的人口密度。 |
| 部署（插脚 && 上 MOD） | 安置物品的行为。玩家通过将共振器部署在据点中来控制据点。     |
| 阵营                   | 两大阵营为争夺控制权而战：反抗军（蓝军）和启蒙军（绿军）。   |
| 入侵（摸 po）          | 从据点中获取物品的途径。不是每一次入侵都能成功               |
| intel 情报地图         | 玩家可以通过该网站查看当前冲突在全球的局势并与其他玩家进行交流。 |
| 道具                   | 包含获得的游戏物体的库存。（本书第六章中会介绍）             |
| Mind Units (MU)        | 用于衡量在一个 Control Field 中生活的人口数量。"INTEL" 视图和 Intelligence Map 中会显示全球的 Mind Unit 分布。 |
| Decay                  | 如果不对 Resonator 进行充能，随着时间流逝，它们的能量会自然而然地衰减，并且会失去 XM 值。当一个 portal 的所有 resonator 都失去 XM 值之后，它将变为中立状态。 |
| Portal MOD             | 一种可以安装到其他物体上以提升后者能量或性能的物体。例如，在 Portal 上安装一个 Shield MOD 可提升该 Portal 的防御能力。 |
| XM（外来物质）         | 从另一空间泄漏到我们宇宙中的一种罕见、强大的三级能量。这种能量为塑造者的所有技术奠定了基础。您必须使用 XM 来启用扫描器。如果 XM 值降到临界级别，您的扫描器将无法使用。您可以通过在这些区域中四处走动来收集 XM（扫描器地图上发光的小球就代表了这些 XM）。您的扫描器会自动收取 XM。 |
| Scanner扫描器          | 扫描器是您手机的核心技术，能够检测出据点并与外来物质 (XM) 以及共振器和 XMP（武器）等 XM 构成设施相互作用。 |

*虽然 ingress 官方有中文翻译，但还是推荐使用英文界面，更加方便 agent 之间的交流*

### 阵营选择

在游戏开始时，您将选择您的阵营。INGRESS 游戏由反抗军与启蒙军两大阵营组成。 您可以在查看初步简介后选择阵营。一旦做出选择，你便无法更改（后续章节将介绍更改阵营）。

[![阵营选择](https://hz-ingress.gitbooks.io/ingress-tutorial/content/guide/basic_training/images/faction-select.png)](https://hz-ingress.gitbooks.io/ingress-tutorial/content/guide/basic_training/images/faction-select.png)

##### 反抗军（蓝军）

抵抗军始终贯彻维护人性的神圣不可侵犯，XM 这种未知的物质必须要以非常严谨的态度去对待。人类至今还未能解明 XM 的大量涌现对世界造成的影响。启示军对 XM 对于人类未来的伤害一无所知，并企图利用 XM 来引发所谓的人类革新，在没有彻底解开 EXOTIC MATTER 的真面目之前，我们将坚持为捍卫人性而战斗。

##### 启蒙军（绿军）

启蒙军坚信，XM 应该得到充分的利用，推动人类的进步和发展。反抗军却把它视作威胁，顽固抵制。我们主张进步，为知识而战。只要人类还没有完全掌握 XM，只要它还没能发挥出真正的潜力，我们将战斗不息。

「UIC 校区附近大多为蓝军—— Resistance，但选择阵容的权利都在你们自己的手里，请慎重考虑，而且请不要受到他人的干扰」

### ingress Agent 快速指南

您可以通过下面的链接获取快速指南手册（pdf 格式）

- [反抗军全套战场指南](https://p5.zdassets.com/hc/theme_assets/764160/200122727/RES_QuickGuideKit__1_.pdf)
- [启蒙军全套战场指南](https://p5.zdassets.com/hc/theme_assets/764160/200122727/ENL_QuickGuideKit_zhHans.pdf)

「此时，已经默认你们可以科学上网，请填写下列表单已加入 UIC-ingress 小组」

<a href="https://goo.gl/forms/nLHCh9yQvbg9aKp73"> UIC-ingress 表单 </a> 

###Agent 准则

我们希望通过 Ingress 打造趣味无限且安全可靠的游戏体验，让所有玩家以及游戏过程中涉及到的真实世界中的每一个人都能享受其中的乐趣。遵循以下常规准则有助于确保你和其他玩家畅享绝佳体验，并且你在玩游戏时不会给其他人带来负面影响。

#### 一、言行高尚

Ingress 是一个体现战略战术、团队合作和良好竞技精神的游戏。我们不仅仅通过 Agent 的 AP 级别或赢得的奖牌数来评判他们，我们更看重的是他们的人格魅力。遵守规则、与人尊重有加并乐于帮助他人是赢得社区尊重的最佳方式。“己之所欲施之于人” 更是 Ingress 的黄金准则。人无完人，但我们衷心希望你能做到身体力行，努力维护你期望他人也共同遵守的行为标准。

Ingress 面向各行各业的玩家。由于所有 Agent 均会受到你在 COMM 和区域中的行动影响，因此某些互动环节在你看来可能无伤大雅或十分有趣，但可能会对大家的游戏体验造成负面影响，尽管这并非你的本意。

请公平竞技并且仅使用官方的 Niantic Labs 软件；请注意，Ingress 专门针对移动设备，让你能够走出去，大胆探索属于自己的世界！*如果你认为其他玩家存在欺诈行为，请通过帮助中心举报涉嫌滥用的行为。*

#### 二、（在游戏中和现实生活中）谦卑有礼

Ingress 的乐趣之一在于与敌对的 Faction 进行抗衡。而与其他许多游戏不同的是，你可能会在现实中遇到游戏中的抗衡对象。因此时刻注意礼貌待人，享受游戏的乐趣，这样大家都能受益无穷。

当你身处相应区域时，可让 scanner 自行进行操作。游戏过程中，跟遇到的其他 Agent 打个招呼不失为礼貌得体的做法。实际上，许多 Ingress 玩家都从双方 Faction 中结识了新朋友。但请注意，正如所有社交情形一样，有些玩家不太喜欢与人交往，如果他们不愿意与你互动，也请你尊重他们的意愿。

请注意：Portal 是供大家公平竞争的游戏资源，任何玩家或 Faction 都没有占领任何一个 Portal 的特权。双方通过竞争对抗来赢得 Portal 的控制权才是其中的乐趣，请勿过于计较或心存敌意。如果你发现自己正处于争夺 Portal 的激烈战斗中，请务必专注于 Scanner。请克制自我，不要大吼大叫、对其他玩家做不文明手势或发生肢体冲突。此外，请勿在未经他人允许的情况下偷拍其他玩家或偷偷录制视频。注意，某些互动环节在你看来可能无伤大雅或十分有趣，但在其他玩家或旁观者看来，情况却可能正好相反。应依据常理做出正确判断，如果旁观者或其他玩家并不想与你交谈，请不要打扰他们。

*如果其他玩家争强好斗、恶意挑衅、刻意保护某个特定 Portal 或者让你在某个区域中感觉不舒服，\**请离开该区域，不要参与其中。***

#### 三、尊重玩家隐私

请注意，如果你选用自己上网时常用的 Codename，那么你可能会给他人留下线索，使其能够追踪到你的个人信息。请尝试在 Google 中搜索你想使用的 Codename，如果搜索结果中出现了任何你不希望让其他玩家发现的信息，请考虑选择更平实普通的 Codename。

请尊重其他玩家的隐私，切勿发布或泄露有关用户身份的其他信息，包括姓名、电话号码、电子邮件地址或实际地址。例如，如果你通过现实生活的交流而得知某人的住址或工作地点，请勿执行以下操作：在 Comm 中公开他们的位置信息；在社交网络中发布相关信息；试图通过故意在其住所或工作地点附近丢弃物品来透露相关信息。除此之外，也不要泄露旁观者或其他人的个人信息。

#### 四、遵守人类世界的规则

富有责任感并恪守最高标准。作为一名 Ingress 特工，你的行动不仅会影响游戏空间，同时也会影响真实世界。因此，请务必熟知这两个世界的共同规则。

> 请留心观察你周围的世界；游戏进程中，你无法预料将会欣赏到哪些美丽风景，也无法预料将会听到何种趣闻轶事。

**如果你不确定自己是否有权进入任何房屋或地区，请考虑寻找其他 Portal。请做出明智的判断并对自己的行为负责。**

时刻维护 Ingress Agent 的声誉并遵循社会规则。



### Portal 和 Inventory

 如果视野内一个 Portal 都没有，寻找 Portal 将成为首要任务。

#### 扩大搜索范围

移动到新的地方然后寻找 Portal。主界面上会有箭头提示临近 Portal 的距离和方向。保持警惕，马上出发。

Portal 往往处于所有人可到达的地方，并且在大型城市里最为密集。Portal 往往有明显的对应实体，例如雕塑，纪念碑，特色建筑，露天壁画，古建筑，以及某些商户。Portal 由人类的才智和创造力而生，向空间散发未知的能量（XM）。

你也可以访问 [Intel Map](http://www.ingress.com/intel) 查看大范围的 Portal 分布。

#### 申请 Portal

如果你不幸处于 Ingress 活动尚未开始的区域，那么请通过申请新的 Portal 来帮助扩展你所在阵营的控制范围。仔细阅读 [Portal 申请要求](https://support.google.com/ingress/answer/3066197)，然后开始[申请 Portal](https://support.google.com/ingress/answer/2808254) 吧！

### Hack：获得道具的方式

通过 Hack 你可以获取道具。你可以 Hack 任何一个 Portal，获得道具的概率取决于 Portal 所属阵营。

#### 如何 Hack

1. 靠近 Portal 直到它处于你的作用范围（Scanner 界面中玩家位置周围的黄色圆）内。
2. 点击 Portal，在 Portal 详情界面中点击 Hack 按钮以尝试获取道具。
3. Hack 结果将会出现在 Scanner 界面底部。点击 OPS 按钮可以查看你的道具仓库。

注意：两次 Hack 同一 Portal 需要等待一段冷却时间。

#### Glyph Hack

最近，Scaner 设备中发现了能使玩家看到一系列 Shaper Glyph 的代码。研究证明使用 Glyph 可增加 Hack 获得的道具数量，但是长期使用这一方法的结果仍然是未知的。

##### 快速指南

释放 Glyph 的能力有有两种方式：自动或者手动。长按 Hack 按钮可以手动触发 Glyph Hack。偶尔在 Hack 时会自动出现高收益的 Glyph（无论你是否长按 Hack），如果你成功完成了这个 Glyph 序列，你将有更高的可能性获得奖励道具。

注意事项：

- **放弃 Glyph Hack**：手动触发的 Glyph Hack 可以通过点击 BYPASS 按钮跳过，转为一次普通的 Hack。自动的 Glyph Hack 可以点击 ABORT 跳过，此时你不会得到任何物品。
- **关于可能性**：Glyph Hack 成功并不能保证你得到更多的奖励道具，它只是增加你获得奖励道具的可能性。
- **准备接受挑战**：Portal 等级越高，Glyph 的个数也越多。低等级 Portal 也许只需要你画两个 Glyph，而更高等级的 Portal 需要画更多的 Glyph。
- **技巧和速度**：你的总体表现由准确度和速度两部分组成。
- **注意 Burnout**：Glyph Hack 和普通的 Hack 受到相同的冷却和过热限制。

要有耐心，慢慢来，享受这个过程。就像任何技能一样，Glyph Hack 需要练习来达到高速和高准确率。

##### 手动触发 Glyph Hack

1. 在 Portal 详情界面长按 Hack 按钮来初始化 Glyph 序列。
2. 仔细观看，记住 Scanner 收到的 Glyph。
3. 在倒计时结束之前重新画出你看到的 Glyph，以增加获得奖励道具的可能性。

你获得奖励道具的可能性随着你的速度和准确度增加而增加。

如果获得了奖励道具，它们会显示在 Hack 结果中。

### 占领 Portal

在 Portal 上放置 Resonator 可以占领 Portal。Resonator 调谐并放大 Portal 处自然出现的 XM 能量，使 Portal 的能量增强。

#### 如何占领 Portal

1. 在某个 Portal 处于操作范围内时点击它。
2. 点击 DEPLOY Resonator 按钮。
3. 选择你想使用的 Resonator 等级，然后点击 DEPLOY。 注意：你只能选择使用小于等于你当前等级的 Resonator，例如你现在为 L2，你只能使用 L1 和 L2 Resonator。

越高等级的 Resonator（从 L1 到 L8）能使 Portal 的能量越强。更高等级的 Portal 被 Hack 时会产生更高等级的道具（Resonator，XMP 和 Shield 等）。更高等级的 Portal 还能连接到更远的 Portal。

单个玩家在每个 Portal 上只能同时 DEPLOY 有限数量个不同等级的 Resonator。如果需要建起更高等级的 Portal，你需要和其他玩家合作。

| Resonator 等级 | 单个玩家可 DEPLOY 的数量 |
| -------------- | ------------------------ |
| Level 1        | 8                        |
| Level 2        | 4                        |
| Level 3        | 4                        |
| Level 4        | 4                        |
| Level 5        | 2                        |
| Level 6        | 2                        |
| Level 7        | 1                        |
| Level 8        | 1                        |

邀请朋友加入，一起占领高等级 Portal 吧！

### 升级 Portal

更强大的 Resonator 能增强 Portal 的能量（和等级）。你可以用 UPGRADE 动作来升级 Resonator。

1. 在 Resonator 详情页面点击 UPGRADE resonator 按钮
2. 在八个 Resonator 中选择一个
3. 选择希望升级到的 Resonator 等级，然后点击 Upgrade 按钮

### 提交新的 Portal

> ~~（1.98.1）版本已经关闭了全球范围内的 portal 申请，因此请等待后续开放申请后再尝试提交新 portal。~~
>
> 目前（1.131.0）版本已经重新开启了全球范围内的 portal 申请，但是要求 agent 级别达到 10 级或以上;
>
> 另，已经开放了审核 portal的窗口，需要 agent 达到 11 级或以上

您可以直接通过侦测器定位、拍照和提交候选 Portal，从而帮助我们拓展游戏领域。

您提交的 portal 应满足[候选标准](https://support.google.com/ingress/answer/3066197?&ref_topic=2799270)。

#### 提交方法：

[![新的portal](https://hz-ingress.gitbooks.io/ingress-tutorial/content/guide/build_portals_and_inventory/images/new_portal.png)](https://hz-ingress.gitbooks.io/ingress-tutorial/content/guide/build_portals_and_inventory/images/new_portal.png)

1. 在 Scanner 中长按你想要候选 Portal 在此显示的地方。向右拖动以选择新 Portal，此时系统会启动设备的相机。
2. `拍摄照片`并进行确认。
3. 在确认位置下，确保候选 Portal 的`位置正确无误`。如果位置不正确，或者您看到了需要位置的消息，请触摸地图并进行拖动，以将标记对准候选据点的所在地。
4. 在名称字段中`输入简短标题`（即建筑物、雕像、艺术品等物体的名称）。
5. 输入有关候选 Portal 的说明 （可选）。您可以使用`说明字段`提供有关候选据点意义和历史方面的其他信息。
6. 触摸发送即可提交你的候选 Portal 以供审核。

### 发现和使用 Passcode

#### 关于 iOS 用户

兑换 Passcode 功能在 iOS 上暂时不可用，请访问 [Intel Map](http://www.ingress.com/intel) 来兑换 Passcode。

#### 寻找 Passcode

使用 Investigation Board 来了解 Ingress 的最新剧情并寻求对 Niantic Project, NIA, XM, Shapers 以及各阵营不同问题的答案。 可以使用隐藏在这些报告之中的 Passcode 来兑换道具（Resonator，XMP 等），XM 或者 AP。

另外，一些官方活动会向到场者赠送包含 Passcode 的卡片，特定的官方周边也会赠送此类卡片。卡片上的 Passcode 一般能够兑换活动徽章。

#### 兑换 Passcode

#### 从 Scanner（仅 Android 设备）

1. 启动 Ingress 应用程序。
2. 点击 OPS 菜单。
3. 在顶部菜单选项中滚动找到 PASSCODE，然后点击 REDEEM PASSCODE。
4. 在屏幕底部输入你的 passcode，然后点击 Submit 兑换。

注意：Passcode 是大小写无关的。

#### 从 Intel Map

1. 在右上方点击 Passcode。
2. 输入你的 passcode，然后点击 SUBMIT 兑换。

#### 错误信息

| 错误信息                                                     | 含义                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Invalid Passcode（Scanner 或 Intel Map 上）                  | Passcode 不正确；在 Intel Map 上还可能由于 Passcode 已过期或者超过最大兑换次数。 |
| Passcode circuitry too hot. Wait for cool down to enter another passcode. | NIA 发现了过于频繁的兑换操作。建议过一段时间再尝试。         |
| Passcode fully redeemed（Scanner 上）或者 Passcode invalid （Intel Map 上） | Passcode 已过期或者超过最大兑换次数。                        |

*可以关注这个 <a href="https://t.me/passcodes"> telegram channel </a>，里面会不定时放出可用的 passcode*

### Capsule

Capsule 是一种掉率 Rare 的容器，能够盛放多个道具，并扔在地上以在 Agent 之间大量交换物品。Capsule 能无限次存入或取出道具，其本身性质不会改变。

### 快速指南

Capsule 里的道具数量会被计入你 Scanner 的库存总数。你不能捡起会导致你道具总数超过库存上限的 Capsule。此外，Capsule 本身也会占用一个额外的库存数量。 当你将一个 Capsule 扔到地上时，它会在一定时间后消失，因此最好和预期的收货人在相同的时间和地点完成交换，以确保 Capsule 被顺利捡取。 当一个道具在 Capsule 里时，它将不能被使用。如 Capsule 里的 XMP 不能 Fire，Portal Keys 不能用于 Link 和远程 Recharge。 当你 Recycle 一个 Capsule 时，你将获得 Capsule 及其内部所有道具 Recycle 能获得的 XM 的总和。 Capsule 可以被循环使用，你可以反复 Load 和 UnLoad 道具无数次。

如何使用 Capsule：

打开你的 Scanner，点击 OPS > INVENTORY，选择 Capsule。在这里，你可以 LOAD，UNLOAD, DROP， 或者 RECYCLE Capsule。

触摸 LOAD 按钮以从你的库存里存放道具到 Capsule，下方会出现一个你库存里所有道具的列表，其中有加号和减号以选择放入到 Capsule 的道具的数量。

当你使用加号增加放入 Capsule 的道具数量的时候，列表的滚动会被锁定，TRANSFER 和 RESET 按钮会被启用。长按加减号可以快速增减数量，TRANSFER 按钮以确认存放道具到 Capsule，RESET 按钮以取消这次存放且重置道具数量为 0。

当你准备好将 Capsule 及其内道具交给其他 Agent 时，触摸 DROP 以将其丢弃到你当前位置。

在你的 Scanner 上触摸地图上的 Capsule，点击 ACQUIRE 以捡起 Capsule。

要将道具从 Capsule 里取出，从 Capsule 菜单里触摸 UNLOAD，然后按照和放入类似的过程取出道具。 

这个就是俗称：垃圾桶 的普通 capsule

![23-Capsules1.png](https://lh6.googleusercontent.com/aNcyq4Qglug0mA_cKu3Fhv0t7R5WfYW-7Tfs1XiSVk3N6gl1UFK7iNFr62lK0jmucTqWtbDoYuHylsnWAKepBA1_pu8ykuYHl7D-PQm1wm5N36i_TN9MWXkCT1iiJqwzUUtNDB85)

~~这个是 ingress 内的通用货币：红桶（MUFG 储存胶囊）~~

![MUFG.png](https://lh4.googleusercontent.com/D9uhoaPeJUychA1EJDiGyHEz31KERQDwSULaYYQA1yo7sIZxM3xvm99xyN3pd9Nqr5cVbJrAFoxiXVgLqyPPjferfpBtq8Lq9193v56FuN8G9SkfT4762JTmuye5HXd0LwR2leEG)



**红桶是 Ingress 与日本三菱金融集团商业合作而催生的道具，它的最特别之处，是可以像“获利息”一样奖励道具。**

每一个红桶也可以容纳 100 件道具，可是别兴致冲冲地喂饱它就算了。它可是个只升不跌的投资组合！只要放道具进去，过些时候红桶就会随机复製这些道具。只要红桶没满，你所投放的“本金”越多，“利息”自然就越丰厚。红桶的复制利息率暂时没有人说得准，总之除了桶外，不管哪种道具都可复制。 经实验证明(笑)，放 95 件道具作本金，平均每天有一件回报。可是当红桶已被道具填满(=100)，或你的道具栏已满(>=2000)，可就没有利息了。

> ##### 红桶小贴士
>
> 把所有非常稀有（VR）的道具全都放进红桶裡。若要用到 Shield，Hack Mod，Ada，Jarvis，到时才拿出来就好，未用到时当然是放在桶里收利息！记得定期检查红桶，并提走利息，慎防爆仓。多存几个红桶，方便把投资分门别类，道具周转就更得心应手了。如果你只有一个红桶，请尽量装进 VR 的道具，并用其他道具补充至 95 个，这样红桶的产出将会达到最大化，但是这样无法控制出产的道具种类。如果你有多个红桶，请每个红桶里面都放进一样的道具，不同红桶之间的道具可以不一样，并尽量装至 95 个，以保证每个红桶都能生产你所需要的物品。
>
> 摘自：<a href="https://lesson.cantonres.com">广蓝《蓝精灵教程》</a>

**当然，它现在已经被量子桶（QuantumCapsule）替代了（我没有找到量子桶的图。。。量子桶的效果和红桶基本相同，再次不再赘述。**



### 進攻與防禦

#### 為 portal 部署護盾

護盾可用來增強 portal 的防禦以抵抗地方陣營的襲擊。護短按照稀有度分為 `COMMON`, `RARE`, `VERY RARE`, `VARYRARE AXA` 。 護盾越稀有，它能夠減緩傷害的能力越強大。防禦度（Mitigation）和黏著度（Stickness）為護盾的兩個量化屬性。如果 portal 上不輸了多個護盾，則總防禦度為各護盾防禦度綜合。

各類護盾的防禦度和黏著度如下表所示：

| 護盾種類  | 防禦度 | 黏著度 | 所需 XM |
| --------- | ------ | ------ | ------- |
| Common    | 30     | 0      | 250     |
| Rare      | 40     | 15     | 500     |
| Vary Rare | 60     | 45     | 1000    |
| AXA       | 70     | 80     | 1000    |

![9-DefenseMods1.png](https://lh4.googleusercontent.com/pqvgwJZllkwtoLmxQtKLHC8GW696yFXplWDRxVgSWnpXLe1_EJ8NnR4c0y-G5eUwxE43XKvkqnl23tHBsvjge7HSn8NG4z7dnQlXkOr4JCDGVH9Ib-wwcqBwiUs4lD3FugYio2En)

#### 反击增益器（Force Amp）

反擊增益器的功能是加強 portal 受到攻擊時的反擊能力。這是一種只有「Rare」的道具。一般而言，單一反擊增益器已經足夠了，多個並沒有太多的疊加傷害。

多個反擊增益器效力遞減如下，部署一個等於兩倍傷害，第二個再增加 0.25 倍的傷害，第三個再疊加 0.125 倍傷害，第四個再疊加 0.125 倍傷害。

![9-DefenseMods2.png](https://lh4.googleusercontent.com/HR_Pgopepz87Kmlc6pQmdQuhinEQEIPUNQdtnTNMeEWUf-5lJ8bRfrN5Otzf-4XowUkp8nuCVKKehF_cFEOAcD6HE_-Vws61M1_ETj1uE7NVmkevRG4N43IOGPzyvR-mBV4M48K9)