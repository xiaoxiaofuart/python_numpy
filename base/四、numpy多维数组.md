1. 项目中引入python数据分析三剑客
:::warning
# 引入数据分析三剑客
import numpy as np
import pandas as ps
import matplotlib.pyplot as plt
:::

2. 查看numpy的版本
:::warning
np.__version__
:::

3. 使用plt读图片，将图片转换为ndarry
:::warning
nd = plt.imread('../bird.jpg')
#三个中括号，表示是一个三维数组
#使用shape属性可以查看数据的描述
nd.shape
#输出为(960, 1200, 3)，960表示数据有960行，1200表示宽度，3表示点的值，括号中有几个数据表示是几维数组
:::
![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703938518018-bcc94cca-0143-4ced-aa5a-24cec94af29a.png#averageHue=%23fcfcfb&clientId=u0a86a7f8-8a72-4&from=paste&height=318&id=u91c3f354&originHeight=398&originWidth=1396&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=37622&status=done&style=none&taskId=u1e0fa989-e90c-44cf-831c-731ad7077b2&title=&width=1116.8)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703939639663-84a35dc5-016f-4088-a7d1-2935beb3eb3e.png#clientId=ub16759fb-e7f8-4&from=paste&height=71&id=u6ac06e60&originHeight=89&originWidth=688&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=5908&status=done&style=none&taskId=uad2dcfd0-fca7-4791-8c0a-d6724c7000d&title=&width=550.4)

4. 显示图片
:::warning
plt.imshow(nd)
:::
![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703940393076-bf883b5a-a2cc-4c6a-ae94-673a747bc4c1.png#clientId=ub16759fb-e7f8-4&from=paste&height=482&id=uaf190c33&originHeight=603&originWidth=1244&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=225264&status=done&style=none&taskId=u992eab62-7a4d-4b04-9e8b-51a142e29ef&title=&width=995.2)
