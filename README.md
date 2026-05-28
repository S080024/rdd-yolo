# rdd-yolo
##  1. 代码依赖关系和需求

### 1.1 实验平台及环境

* **CPU**: Intel(R) Core(TM) i5-9500
* **GPU**: NVIDIA A40
* **Python 版本**: 3.8
* **PyTorch**: 1.10.0

### 1.2 训练超参数

* **Learning rate**: 1e-2
* **Optimizer**: SGD
* **Momentum**: 0.937
* **Weight decay**: 5e-4
* **Close mosaic**: 10
* **Amp**: true
* **Epochs**: 300
* **Batch size**: 8
* **Image size**: 640×640

### 1.3 文件说明

* **模型配置文件存储于**: `RDD-YOLO\ultralytics-main\ultralytics\nn\Add_module`
* **train.py**: 训练模型的脚本
* **val.py**: 使用训练好的模型计算指标的脚本
* **detect.py**: 推理的脚本

## 2. 相关细节

为了充分验证所提出的方法的有效性和泛化性能，本文采用三个数据集进行检测。即：采用NEU-DET数据集进行钢材表面缺陷检测，采用DeepPCB数据集进行PCB缺陷检测。采用自制数据集进行阀杆缺陷检测，相关数据集可从百度网盘链接中获取：

* **百度网盘链接**: *(https://pan.baidu.com/s/19B9GJmhCZJMgHh3oKvhTVg?pwd=kjke )*
* **提取码**: `kjke`
