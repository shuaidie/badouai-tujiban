继续尝试上一周的思路，这一次成功了。有一些改动：
1. 把损失函数改成了二分类交叉熵；
2. 把 learning rate 稍微提高了一点；
3. 把 embedding 的维度提高到30；
4. 对数据维度做了相应的调整。

训练基本收敛，最终能够正确预测。

```python
=========
第1轮平均loss:0.411000
A类样本数量：175, B类样本数量：25, C类样本数量：0
正确预测个数：175 / 200, 正确率：0.875000
=========
第2轮平均loss:0.350486
A类样本数量：164, B类样本数量：36, C类样本数量：0
正确预测个数：164 / 200, 正确率：0.820000
=========
第3轮平均loss:0.244143
A类样本数量：174, B类样本数量：26, C类样本数量：0
正确预测个数：174 / 200, 正确率：0.870000
=========
第4轮平均loss:0.201851
A类样本数量：175, B类样本数量：25, C类样本数量：0
正确预测个数：175 / 200, 正确率：0.875000
=========
第5轮平均loss:0.184732
A类样本数量：170, B类样本数量：30, C类样本数量：0
正确预测个数：170 / 200, 正确率：0.850000
=========
第6轮平均loss:0.156286
A类样本数量：178, B类样本数量：22, C类样本数量：0
正确预测个数：178 / 200, 正确率：0.890000
=========
第7轮平均loss:0.144809
A类样本数量：170, B类样本数量：30, C类样本数量：0
正确预测个数：170 / 200, 正确率：0.850000
=========
第8轮平均loss:0.130259
A类样本数量：168, B类样本数量：32, C类样本数量：0
正确预测个数：168 / 200, 正确率：0.840000
=========
第9轮平均loss:0.114262
A类样本数量：171, B类样本数量：29, C类样本数量：0
正确预测个数：171 / 200, 正确率：0.855000
=========
第10轮平均loss:0.108083
A类样本数量：175, B类样本数量：25, C类样本数量：0
正确预测个数：175 / 200, 正确率：0.875000
=========
第11轮平均loss:0.102845
A类样本数量：168, B类样本数量：32, C类样本数量：0
正确预测个数：168 / 200, 正确率：0.840000
=========
第12轮平均loss:0.099838
A类样本数量：171, B类样本数量：29, C类样本数量：0
正确预测个数：171 / 200, 正确率：0.855000
=========
第13轮平均loss:0.105873
A类样本数量：169, B类样本数量：31, C类样本数量：0
正确预测个数：169 / 200, 正确率：0.845000
=========
第14轮平均loss:0.090542
A类样本数量：172, B类样本数量：28, C类样本数量：0
正确预测个数：172 / 200, 正确率：0.860000
=========
第15轮平均loss:0.082423
A类样本数量：167, B类样本数量：33, C类样本数量：0
正确预测个数：167 / 200, 正确率：0.835000
0 auvxe1 tensor([0.0003])
0 yrw8rg tensor([0.0005])
0 rtw3qg tensor([0.0007])
1 nlhdww tensor([0.9997])
```