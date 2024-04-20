论文地址：[https://doi.org/10.48550/arXiv.1806.08342](https://doi.org/10.48550/arXiv.1806.08342)  

### 摘要

### 介绍

### Quantizer Design

#### Uniform Affine Quantizer (均匀映射量化)  
均匀映射量化公式如下：

<img src="./1.png" width="50%" height="50%">

反量化公式如下：

<img src="./2.png" width="50%" height="50%">

2维卷积公式如下：

<img src="./3.png" width="50%" height="50%">  

#### Uniform symmetric quantizer (均匀对策量化)

<img src="./4.png" width="50%" height="50%">

在SIMD实现中，权重约束为：

<img src="./5.png" width="50%" height="50%">

反量化公式如下：

<img src="./6.png" width="50%" height="50%">

#### Stochastic quantizer（随机量化）