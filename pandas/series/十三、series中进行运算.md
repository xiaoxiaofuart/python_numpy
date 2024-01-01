1. series支持指定的基本运算，同时两个series相加是按照索引下标相同的数组进行相加的，不存在的索引下标会返回nan。可以通过add函数，同时通过fill_value指定默认值
```python
# series中的运算
#基础运算
serials4= pd.Series(np.random.randint(0,50,(5,)))
serials4

serials4+10
serials4*10
serials4/10
serials4//2
serials4**2


# 两个series中进行运算
serials5= pd.Series(np.random.randint(0,10,(3,)))
serials6= pd.Series(np.random.randint(0,10,(4,)))
display(serials5,serials6)


# 两个series相加默认是根据索引下标相同的进行相加，不存在的索引会返回空值
serials5+serials6
#想要保留不存在的下标，可以使用add函数，指定fill_value指定默认值
serials5.add(serials6,fill_value = 0)
```
