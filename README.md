# SD1-1106-

# 基于FCOS的车辆、行人检测任务计划书

## 1.任务简述

- 车辆行驶过程中的周围车辆的感知检测，为后续的自动驾驶任务提供决策基础，部署到移动端设备
- **任务场景**：驾驶过程中的周围车辆检测
- **边界场景**：
  - 光线 日照，每天不同的时间端；
  - 天气 阴天、晴天、雨天；
  - 地理位置 城市、乡村、隧道、高速等
- **1.1检测流程****
  ![流程](imgs/检测流程.png)

## 2.数据集

- baseline 训练及优化使用ONCE（华为）：One Million Scenes for Autonomous Driving数据集( Dataset数据集地址：once-for-auto-driving.github.io/index.html)
- ![ONCE](imgs/oncedataset.png)  ![ONCE_s](imgs/once_.png)
- cited  from  Mao, J., Niu, M., Jiang, C., Liang, H., Chen, J., Liang, X., ... & Xu, C. (2021). One million scenes for autonomous driving: Once dataset. arXiv preprint arXiv:2106.11037.
- 后期使用根据回传的数据进行模型的迭代优化
- **类别数** ： 1类，车辆，选用汽车类
- **15k 全注释场景，5类（汽车、巴士、卡车、行人、骑自行车者）
- 收集图片信息

## 3.评价指标

- 车载目标检测器属于移动端的边缘检测设备
- 要同时兼顾准确率和速度两方面的指标在检测准确的同时以应车辆间相对速度过快等突发情况
- **精度指标** ：mAP
- **实时性指标**：Fps

# 工作安排

- **设备选取**：
- **模型选取**
- **数据集收集**：标注标准
- **代码框架**：工程拆解
  - 数据集处理：模型的输入格式、增强
  - 模型训练
  - 模型优化
- **部署流程：**
  - 部署芯片确定
  - 模型量化及编译
  - 模型部署
- **数据回收 **
  - 报警数据回传
  - 埋点，需要的数据回传
- **模型迭代**


