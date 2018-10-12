<!--
title: 视觉设计指引
-->

# 视觉设计指引

AntV 色板（ 数据可视化色彩体系）是基于 [Ant Design 色彩体系](https://ant.design/docs/spec/colors-cn)，并结合数据可视化特性而设计。
在数据可视化设计中，对色彩的运用应首先考虑准确性，需达到信息传递、操作指引、交互反馈，或是强化、凸显某一个信息的目的，其次是品牌识别性。

选择 AntV 色彩时有以下三个注意点：

- 根据不同的数据特性选择相应的色彩，保证数据传达的准确性；
- 结合当前页面环境，建立视觉连续性；
- 视觉层次清晰可辨，保证色彩足够的对比度的同时更容易被视障碍（色盲、色弱）用户辨别。

## 标准色板

在可视化领域中，数据信息到颜色的映射是非常重要的一个环节，分为色调、饱和度、亮度三个视觉通道。通常色调属于分类的视觉通道，饱和度和亮度通常用于连续的视觉通道。

AntV 色板包含分类色板、连续色板及语义色板，用户选择色板时需对照数据特性选择相应配色方案。

![color](https://cdn.nlark.com/lark/0/2018/png/56/1536551245983-9db7af87-28e2-412d-bd33-1dfb9a63005e.png)

## 扩展色板

![color-extended](https://cdn.nlark.com/lark/0/2018/png/56/1536651057097-d8a11b3d-899c-4f55-a85f-ec5b821a08fe.png)

## 使用指南

我们发现，在提供官方色板的前提下，仍有用户并不是十分擅长在实际场景中应用色板。在此我们提出几个设计指引供参考。

### 避免使用过多的颜色数量

在实际应用中，经常会出现大量颜色使用的误区，建议高亮重要的数据（不超过8个），其他数据默认置灰，通过图例交互进行查看。

![guide-1](https://cdn.nlark.com/lark/0/2018/png/56/1536651320078-7e59d0e8-f5bc-4a34-88e2-8432f92c580a.png)

### 数据映射的规则尽量简单

样的数据，映射规则尽量保持为一种。

例如当使用柱形的高度来映射数据时，就不需要再加上颜色的维度去映射数据了。

![guide-2](https://cdn.nlark.com/lark/0/2018/png/56/1535876613421-b25085a8-312e-4220-905b-17a445a96a20.png)

### 对应数据，做到准确的映射

对应自己的数据，按照数据特性选用对的色板，下图中分类数据应选用分类色板，而不是连续色板。

![guide-3](https://cdn.nlark.com/lark/0/2018/png/56/1535877111908-fb5df5e1-a7f5-4a72-9001-d67ef7fd23c0.png)

### 解释你的颜色

当图表中出现不同颜色是，需要向读者解释颜色代表的含义。<!-- （图例链接） -->

![guide-4](https://cdn.nlark.com/lark/0/2018/png/56/1535877949867-4d5c1e8b-04fe-47c4-98a9-9c0771b014cd.png)

### 上下文保持颜色的一致性

对于统一度量，使用同样的颜色方案，而且在整个页面（通常是仪表盘）使用时，注意保持整体颜色方案的一致性。

![guide-5](https://cdn.nlark.com/lark/0/2018/jpeg/56/1536650305089-bc77ae77-db1b-40d9-ad00-bdd3dc514aad.jpeg)

### 色板可持续升级

定义标准色板不是一件容易的事情，所以我们也一直在努力优化修改，升级后的色板在不久的将来上线，敬请期待。

