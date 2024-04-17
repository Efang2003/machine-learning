# 第一章
## 专业术语
**标记**：学习样本在某个方面表现的潜在规律  
* 取值为离散型：分类任务，标记需*数值化*
* 取值为连续型：回归任务，标记为取值范围

  
**泛化**：对未知事物判断的能力  
**假设空间**：能够拟合训练集的算法模型  
**版本空间**：假设空间的集合  
**归纳偏好**：模型自身对于选择算法的倾向

# 第二章
**误差**：实际预测输出与样本真实输出间的差异  
希望得到泛化误差小的学习器  
**过拟合**：学习能力过强，把训练样本自身特质当做一般特质  
**欠拟合**：学习能力低下，训练样本性质未学好  
## 评估方法
划分训练集与测试集
* **留出法**：将数据集按照比例划分为两个互斥的集合，分层*采样*
* **交叉验证法**:将数据集划分为k个大小相似的互斥子集，然后每次用k-1个子集的并集作为训练集，余下的子集作为测试集，进行k组测试和训练
* **自助法**:每次从数据集中随机选择一个样本，将其拷贝放入新数据集，然后再将其放回原始数据集，使该样本在下次采样时仍保留
## 性能度量
### 回归任务
**均方误差**
### 分类任务
二分法常用：混淆矩阵
* **错误率与精度**
* **查准率，查全率** ：画P-R曲线
   * BEP平衡点，查全率等于查准率时的取值
   * F1度量，也可使用一般形式表达不同偏好
* **ROC曲线**：设立分类阈值
  * AUC为ROC曲线下的面积  
* **代价敏感错误率**
  * 设立一个代价矩阵
  * 画出代价曲线
## 比较检验
### 单个学习器
* **假设检验**
### 多个学习器
* **交叉t检验**
* **Friedman检验与Nemenyi后续检验**
## 偏差与方差
**偏差**：度量了学习算法的期望预测与真实结果的偏离程度  
**方差**：刻画了训练集变动即数据扰动带来的影响  
**噪声**：人工标注数据带来的误差  
  
  
 
