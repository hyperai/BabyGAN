# 用 BabyGAN 预测孩子长相


**BabyGAN** 是一个基于 StyleGAN 的儿童长相预测器，可以基于给定的父母双方图像，预测孩子的长相。  

**主要预测方法为：** 使用基于 GAN 架构的神经网络模型，从输入的父母图像中提取 latent representation，然后用算法将其按一定比例混合，生成孩子图像。  

利用 latency direction，可以改变年龄、面部朝向、情绪及性别等参数。  

- **GitHub 仓库: [BabyGAN](https://github.com/tg-bomze/BabyGAN)**(*创建者: [Denis Malimonov](https://github.com/tg-bomze)*)  

- **神经网络: [StyleGAN](https://github.com/NVlabs/stylegan)** (*创建者: [Tero Karras](https://research.nvidia.com/person/tero-karras), [Samuli Laine](https://research.nvidia.com/person/samuli-laine), [Timo Aila](https://research.nvidia.com/person/timo-aila)*)

- **编码器: [stylegan-encoder](https://github.com/pbaylies/stylegan-encoder)** *(创建者: [Peter Baylies](https://github.com/pbaylies), [Dmitry Nikitko](https://github.com/Puzer))*  


#### 本教程主要演示了：

- 从本地加载训练好的 BabyGAN 模型
- 准备父母双方图像，并获取其 latent representation
- 用模型生成孩子的面容
- 调整孩子的性别、年龄等参数，生成符合需求的孩子图像

**调整孩子性别、年龄等特征的示意动画：**

![](https://tva1.sinaimg.cn/large/008eGmZEly1gpgxgq4c2ng30m00lzkjw.gif)


#### 安装环境：
- Python：3.6
- TensorFlow：1.15

#### 代码目录：
- 准备工作
- 准备父母图像
- 生成孩子图像
- 生成具有某些特征的孩子图像

#### 注意事项：
- 本教程推荐使用 GPU 运行