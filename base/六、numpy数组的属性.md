#ndarray的属性
:::warning
#查看多维数组的描述
a = tu.shape
:::
:::warning
# 查看数组的维度
b = tu.ndim
:::
:::warning
# 查看数组的类型
c = tu.dtype
:::
:::warning
# 查看数组总长度
d = tu.size
a,b,c,d
:::
![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703991141173-d7748d4d-1345-4e65-b0ae-771b362471f5.png#averageHue=%2348a379&clientId=ud114ebce-18a9-4&from=paste&height=231&id=u8465cff4&originHeight=289&originWidth=1406&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=43596&status=done&style=none&taskId=u63c60630-bb74-47a9-b8a5-34b5f5581bf&title=&width=1124.8)

1. 数组索引
:::warning
# 数组的索引
rands = np.random.randint(0,100,(3,4,5))
rands
#h获取最后一个数组元素
a = rands[-1,-1,-1],
b = rands[2,3,4]
rands,a,b
:::

2. 切数组切片
3. 

:::warning
定义一个随机二维数组
randints = np.random.randint(1,10,(5,6))
randints
![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703993675686-9be12185-62de-45ae-b990-cc423f71055c.png#clientId=ud114ebce-18a9-4&from=paste&height=86&id=u71edbca1&originHeight=215&originWidth=1002&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=20175&status=done&style=none&taskId=ue36b05b1-159e-4fbd-9f7e-7aaec22cdea&title=&width=400)

   1. #获取第一行randints[0]

![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703993730715-075fbec4-89cb-4489-ad3b-7c873ed26361.png#averageHue=%23d6b480&clientId=ud114ebce-18a9-4&from=paste&height=89&id=u1d90e9ef&originHeight=97&originWidth=437&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=5727&status=done&style=none&taskId=u0e5c1b5d-918f-4677-bb2d-f5f3510152f&title=&width=400)

   2. 获取第1行和第三行randints[[0,2]]

![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703993768212-bada6023-d56a-4d3d-b402-01599d670eae.png#averageHue=%23faf9f8&clientId=ud114ebce-18a9-4&from=paste&height=99&id=u673f30ab&originHeight=131&originWidth=531&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=13471&status=done&style=none&taskId=ueea177b9-972a-4686-abfe-12fecad55ce&title=&width=400)

   3. 取连续的多行randints[0:3]

![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703993799811-c2219987-b936-47ee-a877-9c3791843669.png#averageHue=%23fbfafa&clientId=ud114ebce-18a9-4&from=paste&height=60&id=ubee02bb1&originHeight=149&originWidth=997&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=18071&status=done&style=none&taskId=ua015311e-7ca0-4138-9a03-68a2bc0f0be&title=&width=400)

   4. 取第一列数据randints[:,0]

![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703993839649-e5f3aef8-bcff-4dc0-ab46-d0ac9f2e5f3e.png#averageHue=%23f9f8f7&clientId=ud114ebce-18a9-4&from=paste&height=75&id=u6cce935d&originHeight=104&originWidth=557&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=8479&status=done&style=none&taskId=u8de84e4d-d1d1-48b8-a1c5-b4326ef4a76&title=&width=400)

   5. 取第二列和第三类列数据randints[:,[1,2]]

![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703993962763-caf7ba01-35b7-4202-bde5-3642039ba998.png#clientId=ud114ebce-18a9-4&from=paste&height=126&id=uaad12493&originHeight=188&originWidth=596&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=12495&status=done&style=none&taskId=u8d63eeed-32a2-40a8-8463-f0e90909261&title=&width=400)
:::

1. 数组反转
:::warning
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
bird = plt.imread('../bird.jpg')
#上下翻转
birdreverse = bird[::-1]
plt.imshow(birdreverse)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703995249158-432ae5dc-e14b-4c9b-97a3-e906c7c26a9f.png#averageHue=%239eaa95&clientId=ud114ebce-18a9-4&from=paste&height=486&id=u08173c06&originHeight=608&originWidth=855&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=216303&status=done&style=none&taskId=u74ebf3fe-e6e0-446d-b5ee-4ec9a4fc33e&title=&width=684)

#左右翻转
bird_down = bird[:,::-1]
plt.imshow(bird_down)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703995276224-3ca00ec4-6a18-481d-b9bd-765088505a32.png#averageHue=%23cbb642&clientId=ud114ebce-18a9-4&from=paste&height=509&id=u82c587d4&originHeight=636&originWidth=1076&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=225393&status=done&style=none&taskId=u4611391c-9d8f-4f7f-ba1b-ecf47599152&title=&width=860.8)

# 对第三个维度进行翻转，颜色进行翻转 RGB->BGR
bird_color_rev = bird[:,:,::-1]
plt.imshow(bird_color_rev)

![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703995298230-eed510a3-b90a-4531-a7a8-f40909505641.png#averageHue=%23eedac9&clientId=ud114ebce-18a9-4&from=paste&height=453&id=ua1e4e640&originHeight=566&originWidth=1018&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=196802&status=done&style=none&taskId=u91916cc8-0773-488f-9011-8ed724c1390&title=&width=814.4)

:::
