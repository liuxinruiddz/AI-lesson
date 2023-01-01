# AI-lesson
AI homework

Homework 1 : Linear Regression
------------------------------
* 数据集`boston.csv`: 波士顿房价集
* 在不使用sk-learn回归器的情况下, 分别实现:
  * 多元回归: `Multiple Regression.ipynb`
  * 多项式回归: `Polynomial Regression.ipynb`
* 实现使用梯度下降算法。
* 使用RMSE和R²进行评估。
* 实现交叉验证，并计算模型误差的偏差和方差。
* 与Sk-learn回归器进行比较: 
  * `Multiple Regression sk-learn.ipynb`
  * `Polynomial Regression sk-learn.ipynb`
  
Homework 2 : Logistic Regression（空）
------------------------------
Homework 3 : AdaBoost
------------------------------
* 数据集`boston.csv`: 波士顿房价集，用于回归练习
* 数据集`mnist_binary.csv`: 二值化处理后的MNIST数据集，用于分类练习
* 在不使用sk-learn的情况下, 实现:
  * AdaBoost分类器: `AdaBoost Classifier.ipynb`
* 使用sk-learn决策树分类器/回归器
* 提供预测概率
* 分类器/回归器评估: roc, auc, r-square, mse
* 与Sk-learn对应的分类器/回归器进行比较: 
  * `AdaBoost Regressor sk-learn.ipynb`
  * `AdaBoost Classifier sk-learn.ipynb`

分析
-------
### 回归器
Multiple Regression: MSE = 33.44897999767652
<br> Polynomial Regression: MSE = 30.82890843966428
<br> AdaBoost Regressor: MSE = 28.40085105292288
* 与线性回归的指标进行对比，相比之下，AdaBoost的均方误差更小，也就是结果更优。虽然 AdaBoost 使用了弱回归器，但是100个弱回归器组合起来而形成的强回归器，效果优于多元回归和多项式回归算法。
### 分类器
* 与决策树分类器的指标进行对比，在经过20个弱分类器之后，AdaBoost的效果明显优于决策树，其优势在于将多个弱分类器组合起来形成强分类器，使整体分类效果得到显著提升。

Homework 4 : XGBoost
------------------------------
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
