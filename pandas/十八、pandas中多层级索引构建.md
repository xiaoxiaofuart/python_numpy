1. pandas中构建多级索引可以分两种方式进行构建
   1. 使用隐式构建的方式进行构建
   2. 使用显示构建的方式进行构建

```python
import numpy as np
import pandas as pd

#构建多级索引有两种方式，第一种隐式构建，第二种显示构建
# 准备数据
data = np.random.randint(60,100,(6,6))
data


#隐式构建
# 指定行级索引
index = [
    ['订单中心','订单中心','订单中心','客资中心','客资中心','客资中心'],
    ['丁一','王二','张三','李四','王五','赵六']
]

#指定列索引

cloums = [['1月','1月','1月','2月','2月','2月'],
          ['质量','需求','自评','质量','需求','自评']
         ]

muti_index = pd.DataFrame(data,index=index,columns=cloums,dtype=np.int16 )
muti_index


#显示构建有多种方式1）通过 
# 通过pd.MultiIndex.from_arrays指定索引
index1 = pd.MultiIndex.from_arrays([
    ['订单中心','订单中心','订单中心','客资中心','客资中心','客资中心'],
    ['丁一','王二','张三','李四','王五','赵六']
])
cloums1 = [['1月','1月','1月','2月','2月','2月'],
          ['质量','需求','自评','质量','需求','自评']
         ]
multi_index1 = pd.DataFrame(data,index=index1,columns=cloums1,dtype=np.float16)
multi_index1



# 通过pd.MultiIndex.from_tuples指定索引
index2 = pd.MultiIndex.from_tuples(
    (('订单中心','丁一'),('订单中心','王二'),('订单中心','张三'),('客资中心','李四'),('客资中心','王五'),('客资中心','赵六'))
)
multi_index1 = pd.DataFrame(data,index=index2,columns=cloums1,dtype=np.float16)
multi_index1


# 通过pd.MultiIndex.from_product指定索引，笛卡尔积不是所有多层级索引都满足,要求第二行的列表必须相同
index3 = pd.MultiIndex.from_product([['订单中心','客资中心'],
     ['丁一','王二','张三']]
)
multi_index3 = pd.DataFrame(data,index=index3,columns=cloums1,dtype=np.float16)
multi_index3
```
