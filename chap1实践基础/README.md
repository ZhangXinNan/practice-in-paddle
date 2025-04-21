
[TOC]


# 第1章 实践基础

- 张量（Tensor）：一种多维数组。
- 算子（Operator, Op）：每个算子有前向和反向计算过程。



## 1.1 如何运行本书的代码
### 1.1.1 本地运行

```bash
# 使用conda创建虚拟环境，python版本为3.9，paddlepaddle版本为3.0。
conda create -n py39_paddle3 python=3.9
# 激活虚拟环境
conda activate py39_paddle3
# 安装paddlepaddle
python -m pip install paddlepaddle==3.0.0 -i https://www.paddlepaddle.org.cn/packages/stable/cpu/

# 查看使用平台
python -c "import platform;print(platform.architecture()[0]);print(platform.machine())"
# 64bit
# AMD64
```
如果使用PyCharm的话，可以点击右下角的Interpreter Settings来设置虚拟环境。

### 1.1.2 代码下载与使用方法

### 1.1.3 在线运行


## 1.2 张量
### 1.2.1 创建张量
#### 1.2.1.1 指定数据创建张量 paddle.to_tensor()
#### 1.2.1.2 指定形状创建张量 paddle.zeros/ones/full
#### 1.2.1.3 指定区间创建张量 paddle.arange/linspace

### 1.2.2 张量的属性
#### 1.2.2.1 张量的形状
* Tensor.ndim 张量的维度
* Tensor.shape 张量在每个维度上元素的数量
* Tensor.shape[n] 张量第n维的大小
* Tensor.size 张量中全部元素的个数

#### 1.2.2.2 形状的改变 paddle.reshape/unsqueeze
#### 1.2.2.3 张量的数据类型 Tensor.dtype/paddle.cast
#### 1.2.2.4 张量的设备位置 place


### 1.2.3 张量与Numpy数组转换 paddle.to_tensor/Tensor.numpy()

### 1.2.4 张量的访问
### 1.2.5 张量的运算

## 1.3 算子
### 1.3.1 算子定义
### 1.3.2 自动微分机制
### 1.3.3 预定义的算子
### 1.3.4 本书中实现的算子
### 1.3.5 本书中实现的优化器

## 1.4 本书中使用的数据集和实现的Dataset类
### 1.4.1 数据集
### 1.4.2 Dataset类

## 1.5 本书中实现的Runner类

## 1.6 小结