* 数据集`boston.csv`: 波士顿房价集，用于回归练习
* 数据集`mnist_binary.csv`: 二分类处理后的MNIST数据集，用于分类练习
* 在不使用sk-learn的情况下, 分别实现:
  * AdaBoost回归器: `AdaBoost Regressor.ipynb`
  * AdaBoost分类器: `AdaBoost Classifier.ipynb`
* 使用sk-learn决策树分类器/回归器
* AdaBoost分类器实现了多类分类
* 提供预测概率
* 分类器/回归器评估: roc, auc, r-square, mse
* 与Sk-learn对应的分类器/回归器进行比较: 
  * `AdaBoost Regressor sk-learn.ipynb`
  * `AdaBoost Classifier sk-learn.ipynb`

分析
-------
Multiple Regression: MSE = 33.44897999767652
Polynomial Regression: MSE = 30.82890843966428
AdaBoost Regressor: MSE = 28.40085105292288
相比之下，AdaBoost 的均方误差更小，也就是结果更优。虽然 AdaBoost 使用了弱回归器，但是100个弱回归器组合起来而形成的强回归器，效果优于多元回归和多项式回归算法。
