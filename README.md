# SD1-1106-

# 基于FCOS的车辆、行人检测任务计划书

## 1.任务简述
- 车辆行驶过程中的周围车辆的感知检测，为后续的自动驾驶任务提供决策基础，部署到移动端设备

- **任务场景**：
- **边界场景**：
  - **1.1检测流程****
    ![流程](imgs/检测流程.png)

## 2.数据集
- baseline 训练及优化使用ONCE（华为）：One Million Scenes for Autonomous Driving数据集( Dataset数据集地址：once-for-auto-driving.github.io/index.html)
- ![ONCE](imgs/oncedatset.png) ![ONCE_s](imgs/once_.png)
- cited  from  Mao, J., Niu, M., Jiang, C., Liang, H., Chen, J., Liang, X., ... & Xu, C. (2021). One million scenes for autonomous driving: Once dataset. arXiv preprint arXiv:2106.11037.
- 后期使用根据回传的数据进行模型的迭代优化

- **类别数 ：** 2类，车辆和

- **训练集图片：**
- **测试集图片：**

- **收集图片信息**

## 3.评价指标

**简述如何根据你选的数据集和任务，定义目标检测器的性能**

- **精度指标 **：mAP
- **实时性指标**：Fps

## 工作安排

- **设备选取：**
- **模型选取**
- **数据集收集：**标注标准
- **代码框架**：工程拆解
- **部署流程**
- **数据回收** **模型迭代**


