# 机器学习中的评价指标

## 分类任务中常见的评价指标

#### 1.准确率

准确率很好理解，给定n个样本，算法模型去预测这n个样本的label,其中有m个样本是预测对了的，那么
<center> acc = $\frac{m}{n}$ </center>
    
#### 2.精确率

精确率主要是衡量模型对于正样本识别的把握的值。考虑一个二分类问题，总共有n个样本，模型对于这n个样本中预测为正样本的数据中，有TP个是预测正确的，FP个是预测错误的，那么

<center> precision=$\frac{TP}{TP+FP}$ </center>

#### 3.召回率

召回率主要是衡量模型对于正样本的召回能力。考虑一个二分类模型，总共有n个样本，其中有p个正样本，其中模型预测为正样本且预测正确的有TP个，是正样本但是模型没有预测出来的有FN个，那么

<center> recall=$\frac{TP}{TP+FN}$ </center>

#### 4.F1

一般我们会用F1来综合衡量一个分类模型的好坏。它平衡了精确率和召回率两个之间的值，计算出一个类似于“平均”的值

<center> F1 = $\frac{2*Percision*Recall}{Percision+Recall}$ </center>

## 回归任务中常见的评价指标



对于n个样本，样本的真实值

<center> y=[$y_1$,$y_2$,$y_3$,...,$y_n$]</center>

算法模型预测为


<center> $\hat y$ = [$\hat y_1$, $\hat y_2$, $\hat y_3$, ..., $\hat y_n$] </center>

#### 5.MAE

<center> MAE = $\frac{1}{n}\sum_1^n|y_1 - \hat y_1|$</center>
    

#### 6.MSE
    
<center> MAE = $\frac{1}{n}\sum_1^n(y_1 - \hat y_1)^2$</center>

