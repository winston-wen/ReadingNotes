# k-NN算法

![img](https://image.jiqizhixin.com/uploads/editor/79cbcd46-a39a-4bf0-b722-3d0758776c51/1522722926386.jpg)

如图，白色的点是测试点，绿色和红色的点是训练点。

超参有：

* 衡量距离的方法
* k值

## 训练阶段

k-NN是个**惰性算法**。它的“训练”只是把数据载入程序的内存空间，有些案例中还需要转化成合适的格式。

## 测试阶段

对每个测试点p，找到与点p**距离**最近的k个点。用这k个点进行**投票**。票数最多的类别就是测试点的类别。

## 缺点

1. 测试时间过长，和训练样本数正相关。
2. 和坐标系相关。
3. 最重要的是，会受到**维度诅咒**（curse of dimensionality）


