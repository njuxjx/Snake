# Snake
This is a Snake game in Java.

这是用Java语言实现的一个贪吃蛇游戏。

## 1st version
游戏总的代码行数差不多是700行。  

游戏中贪吃蛇的头部是一个红色方块，贪吃蛇的身体结点是渐变色的方块。食物是绿色的圆形。  

您可以通过键盘上的方向键或者WASD键来控制蛇的移动。  

在游戏界面按ESC键可以直接重新开始游戏，按空格键可以实现暂停和开始。  

菜单栏的设置菜单可以设置网格以及边框是否可见。游戏界面右边会显示你的当前长度和当前所花时间。  

吃到食物和死亡时都会有相应的音效。  

截图如下：  
![example-image](https://github.com/njuxjx/Snake/blob/master/1st_version/screenshots/Snipaste_2020-12-15_14-52-24.png)
![example-image](https://github.com/njuxjx/Snake/blob/master/1st_version/screenshots/Snipaste_2020-12-15_14-53-12.png)
![example-image](https://github.com/njuxjx/Snake/blob/master/1st_version/screenshots/Snipaste_2020-12-15_14-54-01.png)

第一版游戏界面的宽度（横向的格子数）和高度（纵向的格子数）分别可以通过 Scene 类中的 width 和 height变量来设置，默认两者都是20。  


## 2nd version
此版本更换了蛇的外形，包括蛇头以及蛇身。  

加入了多种食物，每种食物对应的得分不同，不同分值的食物产生的概率不同，原则是分值越高的食物产生的概率越低。加入了记分功能。  

每种食物在产生5秒时间内如果没有被吃掉就会自动移动或者消失。  



## 3rd version
本次对程序结构进行了调整，调整后所有源程序在同一个包xjx下。  

原来的SnakeDemo.java文件基本保持不变，做了一些修改。  

主界面写在了另外一个源文件MainWindow.java中。  

程序主界面进行了重大改变，首先蛇的活动范围增大了一些，然后加入了设置菜单，可以设置游戏背景，蛇身体，蛇头部，速度。  

加入了背景图片，为了让背景显得简洁一点，可以选择是否显示网格。  

菜单栏加入了游戏使用说明，以及关于游戏。  


## 4th version
此版本相对上一版本加入了障碍物，障碍物随机产生，每隔一段时间自动随机移动，障碍物的长度也随机，排列也随机。  

经过本人的相关测试，不排除游戏开始时障碍物出现在你面前导致来不及躲的情况，以及你加速中障碍物改变位置时也可能出现在你面前，所以加速不像上个版本那样，此版本加速有风险。  

同时，为了配合障碍物的出现，游戏加入了蛇发射子弹击毁前进道路上的障碍物的技能。目前每次只能发射一个子弹，不能连续发射多枚子弹。  

子弹通过吃特定的食物获得，食物样子为一把枪。吃得枪每次增加一颗子弹，不增加得分，增加长度。  

子弹产生的概率在所有食物中最低。按Shift键发射子弹。  

## 5th version
对代码进行了一次重构。  

修复部分bug。 

## 6th version
对代码进行了一次重构。

修复部分bug。  

移除长按加速  

移除食物自动刷新  

移除障碍物自动刷新  

加入AI蛇🐍  

注意此版本的游戏地图直接从map目录下读取，你可以按照目录下的txt文件格式设计自己的地图，目录里面已经包含了三个地图  

map.txt格式如下：  

0	0	0	0	0	0	0	0	0	0	0	  

0	0	0	0	0	0	0	0	0	0	0	  

0	0	0	0	0	0	0	0	0	0	0	  

0	0	0	0	0	0	0	0	0	3	3	  

0	0	0	0	0	0	0	0	0	0	0	  

0	0	0	0	0	0	0	0	0	0	0	  

0	0	0	3	0	0	0	0	0	0	0	  

0	0	0	3	0	0	0	0	0	0	0	  

0	0	0	3	0	0	0	0	0	0	0	  

0	0	0	3	0	0	0	0	0	0	0	  

注意，每行的每个字符后面都有一个\t字符，不能包含任何空行。  

其中，0表示这个位置是路，3表示是障碍物，不能有其他数字。


截图如下：  
![example-image](https://github.com/njuxjx/Snake/blob/master/6th_version/screenshots/Snipaste_2020-12-15_21-00-56.png)
![example-image](https://github.com/njuxjx/Snake/blob/master/6th_version/screenshots/Snipaste_2020-12-15_21-01-48.png)
![example-image](https://github.com/njuxjx/Snake/blob/master/6th_version/screenshots/Snipaste_2020-12-15_21-02-14.png)
![example-image](https://github.com/njuxjx/Snake/blob/master/6th_version/screenshots/Snipaste_2020-12-15_21-03-00.png)

##
有问题通过本人邮件联系我  

thexjx@gmail.com
