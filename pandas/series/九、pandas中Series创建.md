1. pandas 中series创建方式有两种，
   1. 一种通过python中list或者numpy中一维数组创建
   2. 另一种是通过python中dict进行创建，其中key就是索引，值就为series中的值
```python
import numpy as np
import pandas as pd

# serials 创建方式
# 第一种，通过list或者ndarry 创建
list1 = [1,2,3,4,5]
serials1 = pd.Series(list1)
serials1
#通过ndarry 创建
randnint1 = np.random.randint(1,100,(2,),dtype=np.int16)
serials2 = pd.Series(randnint1)
display(serials1,serials2)

#pandas的Series分为value和index 两个部分
#获取值
serials1.values
#获取索引
serials1.index
#通过索引获取值
serials1[0]
#修改索引
serials1.index = ['A','B','C','D','E']
serials1.index =list('ABCDE')
serials1
#通过索引修改值
serials1.A = 8
serials1


#通过字典创建Series
dict_ser = {
    'A':1,
    'B':2,
    'C':5
}
dict_pd = pd.Series(dict_ser)
dict_pd
```
