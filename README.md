# Multi-classifier
use 1 versus 1, 1 versus rest and softmax to implement multi-class classification. draw the decision boundary in 2-d data.

分类问题(classification)是机器学习中一个重要的任务，根据类别数的不同，分类问题可以分为二分类问题（是/不是），也可以是多类别问题（即在多个类别中判断输入数据具体属于哪一个类别）。逻辑回归是常用的二分类器，常见的方法是使用one vs one和one vs rest的策略将其改变成多分类器；另一种办法是修改损失函数为softmax损失函数。根据我们的推导，softmax交叉熵损失函数在进行多分类时可以理解为是在训练多个二分类器的组合，只不过因为softmax训练的是类别向量而不是分界面，所以其训练效率得到了很大的提升。

试验结果表明，使用softmax损失函数的策略相较另外两者在保证准确率的前提下确实可以有较高的效率。
