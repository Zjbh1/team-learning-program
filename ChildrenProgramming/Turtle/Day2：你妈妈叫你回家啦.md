﻿# Day02：你妈妈叫你回家啦

## 🔑技能包

别忘了昨天学习的技能哦：


功能 | 指令
---|---
向前走|`t.forward(100)`
向后走|`t.back(100)`
向左转|`t.left(90)`
向右转|`t.right(90)`

---
今天是第二天，主题是【你妈妈叫你回家啦】

![01](https://img-blog.csdnimg.cn/20210709143219268.png)

老师，你在开玩笑？

哈哈，今天的指令确实和回家有关系，叫做【回家指令】，【回家指令】这是个啥？名字起得这么有创意（无聊）吗？难道要让图图回家？

咳咳咳，回答正确，就是一个让图图回家的指令。

## 回家指令介绍

### （1）简介

为什么叫做回家指令呢？这是因为他是通过英文名`home()`翻译过来的，通过这一条指令可以帮助图图回到起点，也就是说，即使你通过指令让图图跑到了千里之外，我也能用这个指令让他回来，是不是一个很6的指令：

![01](https://img-blog.csdnimg.cn/20210709145509558.png)

### （2）格式

那么，这么6的指令可以用来做什么呢？我来举个例子🌰吧：

#### 📺示例1

题目描述：请参考下面图片中的内容，画出一个直角三角形吧：

![02](https://img-blog.csdnimg.cn/20210709145629614.png)

只知道两个直角边分别是80和60，但是另外一条斜边长度不知道，这个时候怎么办呢？

**路人甲：** 不知道哎

**路人乙：** 我是初中生，我学过【勾股定理】可以算

**隔壁小明：** 难道是用`home`指令

是的，隔壁小明真聪明，通过`home`指令就能解决这个问题，最后一条边其实就是图图返回起点走的路：

![03](https://img-blog.csdnimg.cn/20210709145738449.png)

程序如下：

```python
import turtle as t 
 
t.TurtleScreen._RUNNING = True 
t.shape(name='turtle') 
t.forward(80) 
t.right(90) 
t.forward(60) 
t.home()              # 返回起点
t.done()
```
这样，通过`home`指令，让图图自动返回到起点，于是就画出了最后一条边，是不是非常简单，来试试吧！

## 🚀挑战1

题目描述：请参考下面图片中的内容，画出一个钝角三角形吧。

（备注：钝角三角形就是有一个角度数大于90度的三角形）

![04](https://img-blog.csdnimg.cn/20210709145830431.png)

## 🚀挑战2

题目描述：请参考下面图片中的内容，画出对应的图形吧。

![05](https://img-blog.csdnimg.cn/20210709150029917.png)

## 🚀挑战3

有点厉害啊，已经解决了两个挑战了，那么咱们增加下难度吧！

题目描述：请参考下面图片中的内容，画出有一条对角线的正方形吧。

备注1：对角线就是两个相对的角顶点的连接线

备注2：图图回到起点后会自动旋转到水平向右

![06](https://img-blog.csdnimg.cn/20210709150336439.png)

## 🚀挑战4

能做到这里看来你已经掌握`home`指令的诀窍了，既然这样，那就来完成最后的挑战吧。

题目描述：请参考下面图片中的内容，画出一个直角梯形。

备注：上底就是较短的一条边，下底就是较长的一条边

提示：上底、下底、高的长度需要你自己设定，只要能画出类似的直角梯形就可以啦

![07](https://img-blog.csdnimg.cn/20210709151057169.png)



