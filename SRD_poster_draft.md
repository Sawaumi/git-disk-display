# SRD poster draft
## Introduction
### Background

Artificial intelligence applications have been developed extensively in recent years.
Among those, one pivotal area is autopilot (Liu et al., 2019).

现有的大量研究与部署实现更多的着重于工业生产或大型设备的逻辑控制（如自动驾驶汽车），而面向个人场景的小型化开发依然有待探索。
已经完善的部署方案有扫地机器人，酒店送餐机器人等。其大多使用激光雷达，里程计等传感器与特定建图算法对周遭环境建立地图并导航。
当前广泛应用的建图算法，有来自谷歌的开源算法cartographer。其将激光雷达返回的环境地图块与最近获得的环境数据匹配验证，并将验证后的图块插入到适合的位置，
(Hess et al., 2016)其中采用了回环检测优化图块合并产生的累计误差，使用分支定界法优化回环检测的解值搜索。


~~This project aims to modify the existing achievements and develop an autopilot solution for individual users.
Objectives~~

~~Evaluate current autopilot solutions, corresponding algorithms, and hardware foundations.~~

~~Deploy an autopilot system for driving small vehicles.~~

## Metho刀乐gy
硬件采用了（直接自爆）bingda robotics
Use library opencv mediapipe 
AP control
Cartographer mapping


## Results
拼好的高达与AP遥控和建图实现
# 图 图

姿势识别
根据mediapipe库返回的手指关节位置，计算相机画面中手指第一节指节与第二节指节的夹角，判断手指屈伸。可以此快速识别简单手势。混淆矩阵念图
#图图


## Conclusion
### 小型化民用设备。。。
### 新的操控方式与识别。。。
### 爆改轮椅之
同样的系统可适用于实现电动轮椅的避障与自动驾驶，协助驾驶并在紧急情况下，如使用者失能，自动驶往预设地点。

亦或用于家庭药箱，使用wifi遥控，语音控制或手机或通过使用者的手环检测身体情况自动召来，如递送哮喘或心脏病药物。

或用于稍大型底盘，实现向隔离社区居民的物资递送

~~~~