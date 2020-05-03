
# 场景设计说明

<div><p align = "right">设计和素材处理：胡杰<br>Game场景制作：刘文勋<br>其余场景制作：林博恒<br>素材收集：嵇帆</p></div>

根据胡杰同学的设计图，canvas的大小设置为1920&times;1080，大部分场景的组件都很显然，主要是一些按钮，在结算界面的排行榜可以用scrollview来实现，姑且放了一个在上面。下面着重解释Game场景中的组件：

##### canvas

main camera，background都运行在canvas下

##### main camera

游戏运行时的摄影机，玩家观察游戏

##### background

即整个游戏的背景图

##### grid

实际小羊运动的地图

##### reserve

六个玩家的出生地，为zone1-6

##### players

六个玩家，为player1-6

##### stick

摇杆组件

![image-20200503214832064](https://github.com/Haoxuan-Wu/rjgc-qddzz/blob/master/%E5%9C%BA%E6%99%AF%E8%AE%BE%E8%AE%A1/stick1.png)

![image-20200503214901732](https://github.com/Haoxuan-Wu/rjgc-qddzz/blob/master/%E5%9C%BA%E6%99%AF%E8%AE%BE%E8%AE%A1/stick2.png)

大概是这个意思

##### ring

整个摇杆的作用范围

##### dot

摇杆

##### timelaber

时间标签，用来计时

##### minimap

小窗，用来查看全局情况

##### map

小地图

##### camera

小地图的摄影机

##### accelerate

加速技能

##### times

加速可用次数

##### revive

复活技能，

##### times

复活可用次数

##### gameover

游戏结算

##### lose

游戏失败

##### win

游戏胜利

##### backbutton

返回按钮，label是回到大厅







