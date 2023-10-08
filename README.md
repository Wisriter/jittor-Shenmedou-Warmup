# Jittor  计图挑战赛-热身赛

![主要结果](https://s3.bmp.ovh/imgs/2023/08/31/d51a0cbe2069de0a.png)

## 简介

本项目包含了第三届计图挑战赛——热身赛的代码实现。本项目通过在手写数字识别数据集`MNIST`上训练 Conditional GAN（Conditional generative adversarial nets）模型，通过输入一个随机向量 z 和额外的辅助信息 y (如类别标签)，实现了特定数字图像生成。

## 安装 

本项目可在 1张 RTX 3090Ti 上运行，训练时间约为 20分钟。

#### 运行环境

- ubuntu 20.04 LTS
- python >= 3.7
- jittor >= 1.3.0

#### 安装依赖

执行以下命令安装 python 依赖

```
pip install jittor
```

## 训练

可运行以下命令进行训练：

```
python CGAN.py
```

## 推理

推理包含在训练部分代码中，训练完成后进行推理，生成result.png，内容为参赛选手id的手写字体。

## 致谢

此项目基于论文 *A Style-Based Generator Architecture for Generative Adversarial Networks* 实现，部分代码参考了 [jittor-gan](https://github.com/Jittor/gan-jittor)。
