1. numpy多维数组要求数组里面的数据类型必须一致，并且会按照优先级str->float->int进行转型
2. 创建ndarry有五种方式
   1. 使用nd.arry([])直接创建，可以使用dtype指定数据类型
   2. 使用np.ones 创建值为1 的数组np.ones((2,2,3),dtype =np.int16)
   3. 使用np.zeros 创建值为0的数组zeros= np.zeros((2,2,2),dtype = np.int16)
   4. 使用np.eyes创建对角线矩阵eye = np.eye(3,3,k=1,dtype=np.int16)
   5. 使用np.linspace创建等差数列np.linspace(0,100,51,retstep=True,dtype=np.int16)

![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703946011072-9d38ab14-419f-4f75-b9d3-85371cc4d994.png#averageHue=%23fbfaf9&clientId=u219e3995-5338-4&from=paste&height=156&id=u83506f9c&originHeight=195&originWidth=1086&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=18529&status=done&style=none&taskId=ud6b12430-ae02-4491-a44a-8836b46ff22&title=&width=868.8)
