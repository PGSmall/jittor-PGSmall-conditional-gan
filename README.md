# Jittor 计图挑战热身赛 CGAN


![主要结果](result.png)

## 简介
本赛道将在数字图片数据集 MNIST 上训练 Conditional GAN（Conditional generative adversarial nets）模型，通过输入一个随机向量 z 和额外的辅助信息 y (如类别标签)，生成特定数字的图像。

## 安装 
本项目可在 1 张 A100 上运行，训练时间约为 5 分钟。

#### 运行环境
- ubuntu 18.04 LTS
- python >= 3.7
- jittor >= 1.3.0

#### 安装依赖
无特定依赖项

#### 预训练模型
下载预训练模型模型 [`discriminator_last.pkl`](https://drive.google.com/file/d/1CzNiZpcf9OXTRkcS4vDuq5ugbNzBWYya/view?usp=sharing)和[`generator_last.pkl`](https://drive.google.com/file/d/1t8oa925ugg5hrTC14SCzzpVlyD7wnnbf/view?usp=sharing)，放在根目录即可。



## 训练
单卡训练可运行以下命令：
```
python CGAN.py
```

## 推理
训练完毕后，自动生成数字序列。
```
python CGAN.py
```
