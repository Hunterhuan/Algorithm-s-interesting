# 算法的乐趣

空闲时间看了《算法的乐趣》一书，里面讲解有一些比较经典问题的算法。在看的过程中，顺便将代码实现附上。

## Int_to_Chinese

将数字转换为中文数字。

1. 中文数字是每4位为一个unit.
2. 注意“零”的使用

## Chinese_to_Int

将汉字转化为数字。

1. 依次读入汉字，看是权位还是数字。
2. 分别做不同的处理。
3. 注意“零”的转化。

## Pour_Average_water

三个不同容量的水桶通过不同的倾倒来等分8升水的问题。

1. 通过状态树分解，深度遍历得到所有的解法。
2. 中间能记录，防止重复探索，无限循环。

## Cross_the_River

三个和尚和鬼过河的问题。船、左右岸，鬼都不能超过和尚。

1. 类似于上题，通过状态树分解，深度遍历。
2. 中间需要记录，但这次记录只需要记录整个队列的状态就可以了。

## Stable_Matching

稳定匹配问题。

1. Gale-Shapley Algorithm
2. Hungarian algorithm
3. Kuhn-Munkres Algorithm

## Einstein_Question

爱因斯坦的思考题。推断，给定一些条件，推断。

1. 所有状态进行遍历。
2. 判断是否符合条件，如果符合就输出。需要大量计算量。

## TopLogicSort

拓扑排序

1. 计算每个节点的入度
2. 依次输出入度为0的节点，并删除该节点到其他节点的line
3. 循环，直到结束

## Core_path

关键路径

1. 拓扑排序中，计算每个事件的最早完成时间。
2. 计算最晚完成时间
3. 如果一样，则是关键事件。在拓扑排序中依次输出。

## RLE

RLE压缩算法

1. 重复次数+重复单元+重复次数+重复单元
2. 对于非重复的，重复次数最高位标记为0，重复则标记为1
3. 对于压缩图像比较好。

## canlendar

过于复杂，没有实现



## Data_Fitting

很多数据中，如何找拟合曲线

1. 最小二乘法+高斯消元
2. 三次样条曲线拟合（difficult）

## Newton_get_root

牛顿法求方程解

1. 利用微分定义，求方程某地方的导数
2. 找切线与x相交的x坐标。

## Draw_circle

涉及到计算机图形学内容，目前用处不大，之后也可能学到此课程，先不做涉及

## FFT

快速傅里叶

## Big_Int

c++高精度

1. 加减法实现比较简单
2. 乘法也是类似竖式每位相乘
3. 除法采用试商
4. 乘方采用分解法
5. 最大公约数采用Stein算法，也可以用辗转相除
6. 最大公约数*最小公倍数=两数相乘