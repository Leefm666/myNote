## mybatis与hibernate的区别

### mybatis的技术特点

![1561619371125](mybatis的笔记.assets/1561619371125.png)

分页函数：

1. Mysql：limit
2. Oracle：rownum

## Hibernate技术特点

![1561620225540](mybatis的笔记.assets/1561620225540.png)

## 一对一resultType实现

扩展类：order类是order表的模型，要进行和user表多表查询时创建一个orderExe继承order在增加user的属性

![1561625468392](mybatis的笔记.assets/1561625468392.png)

模型有模型：

![1561625590592](mybatis的笔记.assets/1561625590592.png)

![1561626000365](mybatis的笔记.assets/1561626000365.png)

## 一对多

## 多对多

## 延时加载

![1561647820862](mybatis的笔记.assets/1561647820862.png)

## 查询缓存

### ｍｙｂａｔｉｓ的缓存的理解

![1561650217968](mybatis的笔记.assets/1561650217968.png)

![1561650289777](mybatis的笔记.assets/1561650289777.png)

默认一级缓存是开启的是session的

## 二级缓存

![1561650770112](mybatis的笔记.assets/1561650770112.png)

开启二级缓存

![1561651009706](mybatis的笔记.assets/1561651009706.png)

在UserMapper下开启缓存

![1561651255622](mybatis的笔记.assets/1561651255622.png)