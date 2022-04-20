# SRD poster draft
## Introduction
### Background

Artificial intelligence applications have been developed extensively in recent years.
Among those, one pivotal area is autopilot (Liu et al., 2019).

现已完善的部署方案有扫地机器人，酒店送餐机器人等。其大多使用激光雷达，里程计等传感器与
SLAM (Simultaneous Localization and Mapping)算法对环境建图并导航。
当前广泛应用的激光SLAM算法，有Gmapping、hector、Cartographer三种.
但现有的大量研究与部署实现更多的着重于工业生产或大型设备的逻辑控制（如自动驾驶汽车与大型物流仓库的无人驾驶叉车），面向个人场景的小型化开发依然有待探索。

于是我们决定分析比较目前现有的解决方案，算法，硬件与操控系统，并尝试在前人研究的基础上开发一类适用于个人场景的小型化自动导航机器人系统（ROS）。

## Metho刀乐gy
硬件采用了（直接自爆）bingda robotics
Use library opencv mediapipe 
AP control
Cartographer mapping


## Results
Gmapping基于设备的里程计校准扫描得到的地图数据，很难适应不平坦的地面，且没有回环检测
Hector使用高频率的雷达硬件避开了里程计的使用，但雷达成本较高。
而Cartographer将激光雷达返回的环境地图块与最近获得的环境数据匹配验证，并将验证后的图块插入到适合的位置，
(Hess et al., 2016)其中采用了回环检测优化图块合并，从而实现了较前两者更低的累积误差。使用分支定界法优化回环检测的解值搜索，使得低成本雷达也能跑出不错的效果。
拼好的高达与AP遥控和建图实现
# 图 图

姿势识别
根据mediapipe库返回的手指关节位置，计算相机画面中手指第一节指节与第二节指节的夹角，判断手指屈伸。可以此快速识别简单手势。混淆矩阵念图
#图图


## Conclusion
对于低成本的小型化泛用设备来说，使用cartographer算法的单片机系统足以胜任，如果系统能确保在平坦较小室内环境运行，也可以采用Gmapping算法。hector算法并不适用于低成本系统。
### 小型化民用设备。。。
### 新的操控方式与识别。。。
~~~~
