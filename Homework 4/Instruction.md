* 数据集`boston.csv`: 波士顿房价集，用于回归练习
* 数据集`mnist_binary.csv`: 二值化处理后的MNIST数据集，用于分类练习
* 实现:
  * XGBoost分类器: `XGBoost Classifier xgb.ipynb`
  * XGBoost回归器: `XGBoost Regressor xgb.ipynb`
  * GBoost分类器: `GBoost Classifier sk-learn.ipynb`
  * GBoost回归器: `GBoost Regressor sk-learn.ipynb`
* 使用sk-learn决策树分类器/回归器
* 提供预测概率
* 分类器/回归器评估: roc, auc, r-square, mse

分析
-------
### 回归器
Multiple Regression: MSE = 33.44897999767652
<br> Polynomial Regression: MSE = 30.82890843966428
<br> AdaBoost Regressor: MSE = 28.40085105292288
<br> XGBoost Regressor: MSE = 23.854450603698037
* 与线性回归和AdaBoost回归的指标进行对比，相比之下，XGBoost的均方误差更小，也就是结果更优。
### 分类器
* sk-learn实现的GBoost准确度更高。

