1. dataframe创建方式有两种
   1. 直接使用字典的方式创建，key为行级index,value为series
   2. 使用np的二维数组进行创建，通过index指定行级索引，通过columns指定列索引
```python
import numpy as np
import pandas as pd

#pandas创建dataframe有两种方式，第一种通过字典，key为行索引，值为seriesf方式创建
dataframes1 = pd.DataFrame({
    'name':['python','numpy','pandas'],
    'age':[30,10,15]
})
dataframes1


#通过二维数组创建
dataframes2= pd.DataFrame(np.random.randint(60,100,(3,4)),index=['小明','小红','小王'],columns = ['chinese','math','english','chemistry'])
dataframes2

# 可以通过index属性修改行索引
dataframes2.index = ['zhangsan','lisi','wangwu']
dataframes2
#可以通过columns属性修改列属性
dataframes2.columns= ['语文','数学','英语','化学']
dataframes2

```
![image.png](https://cdn.nlark.com/yuque/0/2024/png/33630553/1704115291465-1811f8f3-bb08-4c79-b852-ec6b3537702d.png#averageHue=%23efefee&clientId=u0a9abd92-b127-4&from=paste&height=560&id=u6e624699&originHeight=700&originWidth=911&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=71959&status=done&style=none&taskId=u052f5039-13dc-4af6-a585-a0bacdf849f&title=&width=728.8)
