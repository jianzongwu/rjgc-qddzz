# matchvs调研

![image-20200530214836031](C:\Users\11438\AppData\Roaming\Typora\typora-user-images\image-20200530214836031.png)

所找到的文档的很多图片显示不出以及链接点不进去，且服务开启不了。

所以新问题出现了，是该换个服务器方案还是继续使用matchvs。

以下是matchvs的调研部分。

## 开启服务

打开cocos creator，选择菜单栏 -> 面板 -> 服务，打开服务面板，在列表中点击machvs选项，先为游戏工程设定cocos appid

![image-20200529113152613](C:\Users\11438\AppData\Roaming\Typora\typora-user-images\image-20200529113152613.png)

然后就可以把matchvs sdk集成到项目中。

## 游戏运行逻辑

使用gameserver框架，把客户端的数据传送到服务器端，由服务器端进行结果分析发还客户端。这样就可以大大降低服务端代码的复杂性。

### api

获取实例

初始化：调试环境(alpha)和正式环境(release)

注册，登录，加入房间，组队，房间关闭，离开房间，游戏登出，反初始化

**游戏数据传输**：当玩家在同一个房间时，即可互相通信。开发者可用该接口将数据发送给其他玩家，Matchvs默认将数据广播给当前房间内除自己以外的所有用户。所以我的想法是把每个玩家的输入发送到服务器，服务器结合此时地图的具体情况，给出判断结果，把这个结果发给每个玩家，客户端自己对地图进行渲染。有两个sdk接口，分别是sendevent和seneventnotiy。至于应该发送什么数据结构应该开发者自己协调。

## 两个实例

第一个是斗地主，可以看一下gameserver部分，因为它的client部分是用typescript写的。https://github.com/matchvs/Poke

第二个是贪吃星球，可以看一下client和server的交互。https://github.com/matchvs/demo-creator-gameServer-JS

### 资费说明

预付费模式

后付费，每天24点进行结算

预付费，按套餐计算

