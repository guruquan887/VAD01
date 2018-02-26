# VAD01

欢迎来到VAD01 GitHub。

## 安装
请安装GitHub Desktop进行VAD01项目协同开发管理
建议安装Sublime Text进行VAD01项目开发编辑
\\Apollo采用bazel作为代码编译构建工具，编译c++代码
\\每个源码文件夹下有一个BUILD文件，作用是按照bazel的格式来编译代码
\\OS:Ubuntu Linux 14.04

## 文档
顶层文档架构要求如下，
**每项子集文档参考apollo-2.0.0文档树**：
[00硬件]
   ┝[00车型](00硬件/00车型/):应用场景车型
   ┝[01NVIDIA](00硬件/01NVIDIA/)：英伟达快速开发套件JETSON TX1&TX2
   └[02BOSCH](00硬件/02BOSCH/)：线控厂家博世相关信息
[01需求分析]
   ┝[docs](01需求分析/docs/)此目录下可以找到VAD01文档
       ┝[standards](01需求分析/docs/standards/):法规标准
       ┝[FAQs](01需求分析/docs/FAQs/):常见问题
       └[specs](01需求分析/docs/specs/):VAD01 v1.0 技术文档
   ┝[modules](01需求分析/modules/)：模块化设计
       ┝[calibration](01需求分析/modules/calibration/):标定校准模块
      *┝[canbus](01需求分析/modules/canbus/):CAN总线，收发指令，控制底盘并反馈状态
       ┝[common](01需求分析/modules/commmon/):公有的源码模块
      *┝[control](01需求分析/modules/control/):主控制模块 ，基于车道规划和车辆当前状态，输出转向、加速和制动控制信号到CAN卡
       ┝[data](01需求分析/modules/data/):收集、存储、处理收集到的各种数据
       ┝[dreamview](01需求分析/modules/dreamview/):一个Web应用，帮助用户随时掌握系统的输出数据，包括车道、位置、车身等情况
       ┝[drivers](01需求分析/modules/drivers/):CAN卡、雷达、GPS等驱动程序
       ┝[e2e](01需求分析/modules/e2e/):端到端的深度学习  
       ┝[elo](01需求分析/modules/elo/):百度的车辆自身定位，前向摄像头、全球定位系统、百度高精地图      
      *┝[localization](01需求分析/modules/localization/):车辆定位服务
      *┝[map](01需求分析/modules/map/):地图      
       ┝[monitor](01需求分析/modules/monitor/):监测硬件状态及整个系统的健康程度  
      *┝[perception](01需求分析/modules/perception):障碍物和红绿灯等交通信号感知
      *┝[planning](01需求分析/modules/planning/):根据车辆位置和车辆状态、地图、障碍物、导航信息等计算具体的车道
      *┝[prediction](01需求分析/modules/prediction/):计算障碍物的可能轨迹
      *┝[routing](01需求分析/modules/routing/):路径规划，根据地图和起点终点位置计算出具体的导航信息
       ┝[third_party_perception](01需求分析/modules/third_party_perception/):第三方感知
       └[tools](01需求分析/modules/tools/):通用监控与可视化工具
   ┝[third_party](01需求分析/third_party/)：第三方插件
   └[tools](01需求分析/tools/)：
[02详细设计书]
[03源代码]
[04测试式样书兼报告书]
[05机能实现图]

**文档模版**
(01需求分析/)《00-Document Name-v1.0-(Drafter)-(Project No)-YYYY-MM-DD.doc》

## 咨询

非常欢迎您随时提出疑问或提交bug报告

## 版权


## 免责声明
请参考免责声明
