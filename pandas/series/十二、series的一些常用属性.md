1. pandas中一些常用的属性
   1. shape用于查看series的长度
   2. head与tail用于查看元素的前几行或者后几行的内容
   3. isnull 与 isnotnull 判断元素是否有为空的情况
   4. serires1[~series1.isnull()]用于元素中进行剔重
```python
#series的一些常用属性

# 1.shape属性,返回的时一个元组类型，表示的是series的长度
serials3.shape
#2. head 与tail 属性，工作中经常使用，用来表示查看series前几行或者后几行，默认查看前五行
serials3.head()
#查看后两行
serials3.tail(2)
# pnumpy中np.nan 表示为空，可以用isnull或者isnotnull函数进行判断
serials3['pandas'] =np.nan
serials3
null_if = serials3.isnull()
#进行数据过滤，
serials3[~null_if]
```
