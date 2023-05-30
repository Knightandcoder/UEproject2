# 游戏模式  第二次课作业

链接：https://pan.baidu.com/s/1ZPND89mr7_mvkCGXbnW8EA 
提取码：kksk 


### 倒计时与弹结算UI：


​			 **新增蓝图BP_time, 新增控件ResultGame， 在MyHUD控件加入了倒计时的显示**



  （实现上： 蓝图BP_time，直接加入场景, 主要用于倒计时, 以及倒计时结束时弹出ResultGame的UI。

delay20s后正式开始游戏的60s倒计时，这delay的20s用来等待其他玩家加入，在这20s期间不可射击，delay20s后正式开始游戏的60s倒计时，通过组播游戏的时间来实现玩家游戏时间的同步）





### 物体的初始化、移动与受伤：



​			**新增movingobj文件夹，在其下创建actor：mov   正方体 ，并做了移动的逻辑与受到伤害的逻辑。 在BP_Projectile里修改子弹命中物体（Hat，movobj还是其他）的逻辑** 



（实现上：mov在targetpoint处初始化，设置缩放、平移与旋转的逻辑，并每隔几秒，转换移动方向，该物体标签为movobj（在BP_Projectile里用到，用于判定射击命中））

ps：在击打到移动物体后，左上角会print 小蓝字   “+1”















