1. pandas中concat，默认是进行列合并，可以通过axis属性进行调整，合并时默认相同的列会合并到一起，不通的列会补nan
```python
import numpy as np
import pandas as pd

# 定义一个函数用于生成表格数据
def generate_arry(input_list:list,row_nindex:int):
    return_list = []
    for item  in input_list:
        row_list =[]
        i =0
        while i < row_nindex:
            row_list.append(item+str(i))
            i =i+1
        return_list.append(row_list)
        row_list=[]
    return return_list

# 定义第一个表格
data1 = generate_arry(['A','B','C'],3)
df1 = pd.DataFrame(data1,['小明','小红','小黄'],['A','B','C'])
df1

# 定义第二个表格
data2 = generate_arry(['A','B','D'],3)
df2 = pd.DataFrame(data2,['猴子','小猫','小狗'],['A','B','D'])
df2

# 使用concat对两个表格进行合并,默认是进行列合并,相同的行会合并，不同的行默认会补nan
pd.concat([df1,df2])

#指定进行行合并,默认会合并项同行，不通的行不存在的列会补nan
pd.concat([df1,df2],axis= 1)
```
![image.png](https://cdn.nlark.com/yuque/0/2024/png/33630553/1704296126108-b596c895-9a18-4403-9305-e2bbc7bae2aa.png#clientId=u579a486c-091f-4&from=paste&height=450&id=ue4675fa7&originHeight=563&originWidth=1161&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=46364&status=done&style=none&taskId=u93426806-bf7c-4e1c-8cb1-65e160a9419&title=&width=928.8)
