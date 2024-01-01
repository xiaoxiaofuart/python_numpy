1. series的切片也分为两种
   1. 隐式切片，通过索引下标进行切片，左闭右开
   2. 显示切片，通过索引名称进行切片，左闭右闭
```python
#series的切片也分为两种，显示切片与隐式切片
serials3 = pd.Series({
    'math':100,
     'chiese':110,
     'english':90,
     'python':135,
     'numpy':120,
     'pandas':150
})

#隐式切片,左闭右开
serials3[0:3]
serials3.iloc[0:3]

#显示切片,左闭右闭
serials3['chiese':'python']
serials3.loc['chiese':'python']
```
