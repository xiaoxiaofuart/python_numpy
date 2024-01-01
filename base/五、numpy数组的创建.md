1. numpy多维数组要求数组里面的数据类型必须一致，并且会按照优先级str->float->int进行转型
2. 创建ndarry方式
   1. 使用nd.arry([])直接创建，可以使用dtype指定数据类型
   2. 使用np.ones 创建值为1 的数组np.ones((2,2,3),dtype =np.int16)
   3. 使用np.zeros 创建值为0的数组zeros= np.zeros((2,2,2),dtype = np.int16)
   4. 使用np.eyes创建对角线矩阵eye = np.eye(3,3,k=1,dtype=np.int16)
   5. 使用np.linspace创建等差数列np.linspace(0,100,51,retstep=True,dtype=np.int16)

![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703946011072-9d38ab14-419f-4f75-b9d3-85371cc4d994.png#averageHue=%23fbfaf9&clientId=u219e3995-5338-4&from=paste&height=156&id=u83506f9c&originHeight=195&originWidth=1086&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=18529&status=done&style=none&taskId=ud6b12430-ae02-4491-a44a-8836b46ff22&title=&width=868.8)

   6. 通过arange函数创建，只能创建一维数组ranges = np.arange(100,dtype= np.int16)
   7. 通过np.random.randint创建多维数组np.random.randint(5,10,(10,),dtype=np.int16)，第一个参数表示开始数字，第二个参数表示结束参数，第三个参数表示数组的维度，第四个参数表示数组的形状

![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703989815204-c7fed592-e233-4072-a818-d80e76817f86.png#averageHue=%23d2ae7c&clientId=u04260cc7-2c8d-4&from=paste&height=86&id=ub428b397&originHeight=107&originWidth=1381&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=16497&status=done&style=none&taskId=u48da556a-ff7b-492a-a205-dcc887b6186&title=&width=1104.8)

   8. 创建一个符合正态分布的数组np.random.normal(loc=100,scale= 10,size =(5,5))

![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703990394326-6831146b-efea-4a1d-be52-02fc39e00ed2.png#averageHue=%23fbf9f8&clientId=u04260cc7-2c8d-4&from=paste&height=235&id=u864272fb&originHeight=294&originWidth=1124&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=44799&status=done&style=none&taskId=ubff36d3e-da00-4065-84be-43bae73176f&title=&width=899.2)

   9. 使用np.random.random 或者np.random.rand创建随机多维数组

