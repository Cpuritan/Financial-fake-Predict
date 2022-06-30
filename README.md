# Financial-fake-Predict
近年来不时出现上市公司财务数据造假及暴雷的情况。面对上市公司多年的财务数据报告，筛选数据指标进行跟踪分析和研究，识别真伪，避免投资踩雷🤣。谁造假谁是是是🐱‍🐉😒

本次项目源于泰迪杯数据挖掘挑战赛国二，代码未能较好包装略显凌乱。

### 数据
基于https://www.tipdm.org:10010/#/competition/1354705811842195456/question 的三个问题

本项目基于初始的行业分类，在此基础上又将其划分到，制造业，服务业，文娱行业，传统行业四个行业进行分析，行业重组如下
![image](https://github.com/Cpuritan/Financial-fake-Predict/blob/master/industry.png)

缺失值填补通过剔除和KNN缺失值填补结合。

### 模型
同时部分应用迁移学习思想，发掘不同行业的共同影响特征
![image](https://github.com/Cpuritan/Financial-fake-Predict/blob/master/transf.png)

主要是基于xgboost,randomforest,svc等机器学习模型，并结合stacking构建集成模型,部分调参如下
![image](https://github.com/Cpuritan/Financial-fake-Predict/blob/master/funetuning.png)
