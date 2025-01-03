# 导航
!!! note "可以联系到军事理论导弹部分"



将运载体从起始点引导到目的地的技术或方法称为 导航



导航系统功能

- 测量定位 感知运载体的姿态、位置、速度、方向等信息
- 航行决策 决定运载体运动的方向、速度
- 路径规划 确定运载体从当前位置到达目的地的可行路径或最优路径



导航系统是机器人的“眼睛”和“地图”





## 卫星导航系统

### GPS
GPS即全球定位系统（ Global Positioning System ）。 简单地说，这是一个由覆盖全球的 24 颗卫星组成的卫星系统。这个系统可以保证在任意时刻，地球上任意一点都可以同时观测到 4 颗卫星，以保证卫星可以采集到该观测点的经纬度和高度，以便实现导航、定位、授时等功能。
![](https://philfan-pic.oss-cn-beijing.aliyuncs.com/img/20240925003237.png)



## 多普勒导航
多普勒导航系统是利用多普勒效应 实现的，
该系统由 **磁罗盘或陀螺仪表** 、 **多普勒雷达** 和 **导航计算机** 组成。

多普勒雷达不断地沿着某方向向地面发出无线电波，利用飞行器和地面有相对运动产生多普勒效应，测出雷达发射的电磁波和接收到的回波的 频率变化 ，从而计算出飞行器相对于地面的飞行速度，速度的方向就是该点航线的方向。

![](https://philfan-pic.oss-cn-beijing.aliyuncs.com/img/20240925003725.png)


!!! note "pros & cons"
    === "优点"
        自主性好，反应快，抗干扰性强，测速精度高，能用于各种气候条件。
    === "缺点"
        a.隐蔽性不好 ;
        b.系统工作受地形影响；
        c.测量有积累误差。

## 惯性导航系统 (INS)

- 分类：平台式惯导系统 & 捷联惯导系统
- 模块：计算机、加速度计、陀螺仪或其他运动传感器的平台
- 原理：通过测量机体的加速度和角速度，计算出机体的位置、速度和姿态，实现定位导航

![](https://philfan-pic.oss-cn-beijing.aliyuncs.com/img/20240925003530.png)


!!! note "pros & cons"
    === "优点"
        a. 不依赖外界任何信息实现完全自主的导航；
        b. 隐蔽性好；
        c. 不受外界干扰；
        d. 不受地形影响；
        e. 能够全天候工作。
    === "缺点"
        系统精度取决于单个传感器精度，实际空间位置的漂移是不可避免的，并随时间累积。

## 图形匹配导航系统

与预先的电子地图匹配位置，实现导航

单纯的图形匹配导航不能提供地理坐标位置， 必须和其他导航方式进行组合。更多的是和图形/惯性组合。

图形匹配导航可分为 地形匹配导航和景像匹配导航 两种。

优点： 没有累积误差，隐蔽性好，抗干扰性能较强。


缺点：
a.实时性受到制约；
b.工作性能受地形影响；
c.受天气影响；
d.飞行器的机动性。

无线电跟踪系统

## 地磁导航
地磁场是矢量场，在地球近地空间内任意一点的地磁矢量与其它地点的地磁矢量是不同的，且与该地点的经纬度是一一对应的。因此，理论上只要知道该点的地磁场矢量就可实现全球定位。


优点： 无源、无辐射、隐蔽性强，不受敌方干扰、全天时、全天候、全地域、能耗低的优良特征，导航不存在误差积累，在跨海制导方面有一定的优势。


缺点：
a.地磁匹配需要存储大量的地磁数据；
b.实时性与计算机处理数据的能力有关

## 组合导航系统
组合导航常以 INS 作为主导航系统 ，而将其他 导航定位误差不随时间积累的导航系统，如无线电导航、天文导航、地形匹配导航和卫星导航等系统
作 为辅助导航系统




INS / GPS 组合导航系统：GPS的低动态、窄带宽、高精度；INS的高动态、宽频带、误差慢漂移特性

惯导 / 多普勒组合导航系统

惯导 / 地磁组合导航系统

惯导 / 地形匹配组合导航系统

GPS / 航迹推算组合导航系统