1. dataframe的运算可以为基本的运算
2. 也可以通过两个dataframe进行运算
3. 还可以通过dataframe与series进行运算，默认是进行行相加，可以通过add函数指定axios进行运算
```python
#dataframe的运算
dataframes4 = pd.DataFrame(np.random.randint(60,100,(3,6)),index = ['李六','赵七','吴八'],columns = ['语文','英语','数学','历史','政治','物理'])
dataframes5 = pd.DataFrame(np.random.randint(60,100,(3,6)),index = ['李六','赵七','吴八'],columns = ['语文','英语','数学','历史','政治','物理'])
display(dataframes4,dataframes5)

#基本运算
dataframes4 +1
dataframes4*10

#两个datafram相加,行索引名称必须相同
dataframes4+dataframes5

# dataframe 与 series 操作，默认是进行列相加
series1 = pd.Series([1,2,3,4,5,6],index =dataframes5.columns )
dataframes4+series1

#指定为行相加,通过axios指定
series2 = pd.Series([1,2,3],index =dataframes5.index )
dataframes4.add(series2,axis = 0)
```
![image.png](https://cdn.nlark.com/yuque/0/2024/png/33630553/1704119042024-2b2b02a8-de04-45e5-9971-c819d30fb093.png#averageHue=%23f4f3f3&clientId=u5f116ec8-799e-4&from=paste&height=801&id=u40bff77d&originHeight=703&originWidth=702&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=75102&status=done&style=none&taskId=u640c4d7c-13a6-427b-947b-ac20247ce08&title=&width=800)
