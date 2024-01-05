> jupyter有两种运行模式：命令模式（enter进入）与编辑模式（esc进入）


1. 编辑模式：
   1. ctrl +enter 运行当前单元格代码
   2. shift+enter 运行当前单元格，并且指向下一单元格
   3. alt+enter运行当前单元格，并且在下放新增一个单元格
   4. 

2. 命令模式
   1. ctrl +enter 运行当前单元格代码
   2. shift+enter 运行当前单元格，并且指向下一单元格
   3. alt+enter运行当前单元格，并且在下放新增一个单元格
   4. Y进入代码模式
   5. M进入markdown模式
   6. DD删除所选的行
3. jupyter 中可以使用一些魔法变量对程序进行处理
   1. %run 文件名称  可以实现运行py脚本

![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703929403294-cd960cae-aca1-4e8c-a8d0-a76d29505694.png#averageHue=%23f9f9f9&clientId=u554a3baf-f54d-4&from=paste&height=75&id=u723a89d3&originHeight=94&originWidth=1392&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=7322&status=done&style=none&taskId=u23ab1584-3bf0-4add-a085-eabb7914781&title=&width=1113.6)

   2. 也可以使用 import 运行

![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703929752859-249586bb-409c-4cda-8a62-26f1fefb5b30.png#averageHue=%23fafaf9&clientId=u554a3baf-f54d-4&from=paste&height=95&id=u0715bdf7&originHeight=119&originWidth=1439&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=7953&status=done&style=none&taskId=u2d0b62cc-f70a-4c76-818d-e23808ab046&title=&width=1151.2)

   3. 用于函数统计耗时的命令%time或者%timeit 其中time是用于统计耗时较长的函数，timeit用于统计耗时较短的函数

![image.png](https://cdn.nlark.com/yuque/0/2023/png/33630553/1703930536347-94a11d11-48ea-4359-a96e-9c5c138ecd2c.png#averageHue=%23f9f9f8&clientId=u554a3baf-f54d-4&from=paste&height=292&id=ubbc95be1&originHeight=365&originWidth=1411&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=42687&status=done&style=none&taskId=u881459d6-f410-41ad-b5a4-9dd7559100e&title=&width=1128.8)
