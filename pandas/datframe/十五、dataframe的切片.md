1. dataframe的切片与二位数组的切片类似，优先进行行切片

```python
# dataframe的切片
dataframes3 = pd.DataFrame(np.random.randint(60,100,(3,6)),index = ['张三','李四','王五'],columns = ['语文','英语','数学','历史','政治','物理'])
dataframes3

#进行行切片，获取张三
# 进行隐式切片,左闭右开
dataframes3.iloc[[0]]
dataframes3[0:1]
#进行显示切片，左闭右闭
dataframes3['张三':'李四']
dataframes3.loc[['张三']]


# 进行列切片
#隐式切片
dataframes3.iloc[:,1:3]
dataframes3.iloc[:,[1,3]]
#显示切片
dataframes3.loc[:,['语文']]
dataframes3.loc[:,'语文':'数学']
```
![image.png](https://cdn.nlark.com/yuque/0/2024/png/33630553/1704117421478-88d42148-ce9e-4ce0-b59a-c29055ae14b4.png#averageHue=%23eeeeed&clientId=ufa5d3e7c-8e8d-4&from=paste&height=556&id=ud3170692&originHeight=695&originWidth=1051&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=50778&status=done&style=none&taskId=ueb6b089a-ea06-4078-b3ec-bc77eae2b0f&title=&width=840.8)
