# 遗传算法相关

工欲善其事，必先利其器。

先从基本概念和步骤提起。

## 遗传算法：

一类借鉴生物界的进化规律即优胜劣汰的机制演化而来的一种随机化搜索方法。

## 基本步骤：

* 初始化(设置进化代数计数器，设置最大进化代数，随机生成M个个体作为初始群体)
* 个体评价（计算群体中各个个体的适应度）
* 选择运算（将选择算子作用于群体。就像交配遗传）
* 交叉运算（将交叉算子作用于群体。核心作用的就是交叉算子。）
* 变异运算（将变异算子作用于群体，就像遗传过程中基因可能会变化。）
* 终止条件判断，判断是否出现了最大适应度个体。即所求最优解。

![没了。](https://github.com/doordiey/other_algorithm/blob/master/image/GA.jpg)

其中，对上述步骤的个别名词进行说明。

适应度：各个个体对环境的适应程度叫做适应度。并引用适应度函数来计算个体在群体中被使用的概率。

选择算子：即择优录取，建立在个体适应度评估基础上。（常用的有：适应度比例方法、随机遍历抽样法、局部选择法。

交叉算子： 就类似于生物遗传基因的重组。类似于那个生物的孟德尔的那个遗传定理。就可以将两个个体随机交换某些基因。具有较好的全局搜索能力。

变异算子：引入变异算子使算法具有局部的随机搜索能力。对群体中的个体里的基因值作变动。

终止条件：预期要达到的效果。

## 应用实例：

- 1.函数取最大值问题。
  - 相关代码：[code/GA](https://github.com/doordiey/other_algorithm/blob/master/code/GA/GA.py)

其他应用实例后续更新。











