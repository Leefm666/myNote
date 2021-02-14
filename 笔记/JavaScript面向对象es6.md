# es6中的类和对象

类 class

![1566825121409](Untitled.assets/1566825121409.png)

![1566825485924](JavaScript面向对象es6.assets/1566825485924.png)

![1566825648569](JavaScript面向对象es6.assets/1566825648569.png)

# 类中添加共有的方法

![1566825860603](JavaScript面向对象es6.assets/1566825860603.png)

+ 类中不需要写function关键字
+ 多个函数方法之间不需要添加逗号分隔

# 继承

![1566826119395](JavaScript面向对象es6.assets/1566826119395.png)

super

![1566826458154](JavaScript面向对象es6.assets/1566826458154.png)

# super关键字

![1566826662197](JavaScript面向对象es6.assets/1566826662197.png)

![1566826749354](JavaScript面向对象es6.assets/1566826749354.png)

![1566826828607](JavaScript面向对象es6.assets/1566826828607.png)

![1566871127574](JavaScript面向对象es6.assets/1566871127574.png)

# 使用类的两个注意点

![1566871327815](JavaScript面向对象es6.assets/1566871327815.png)

# this的指向问题

![1566874399487](JavaScript面向对象es6.assets/1566874399487.png) 

# 构造函数和原型

![1566876612808](JavaScript面向对象es6.assets/1566876612808.png)

![1566876642336](JavaScript面向对象es6.assets/1566876642336.png)

![1566876656767](JavaScript面向对象es6.assets/1566876656767.png)

![1566876697540](JavaScript面向对象es6.assets/1566876697540.png)

![1566876735045](JavaScript面向对象es6.assets/1566876735045.png)

![1566876786240](JavaScript面向对象es6.assets/1566876786240.png)

# 静态成员和实例成员

![1566876861645](JavaScript面向对象es6.assets/1566876861645.png)

![1566876989209](JavaScript面向对象es6.assets/1566876989209.png)

# 构造函数原型对象

 ![1566877145138](JavaScript面向对象es6.assets/1566877145138.png)

![1566877794095](JavaScript面向对象es6.assets/1566877794095.png)

一般情况下，我们的公共属性定义到构造函数里面，公共的方法我们放到原型对象上

# 对象原型

![1566879697014](JavaScript面向对象es6.assets/1566879697014.png)

![1566879747095](JavaScript面向对象es6.assets/1566879747095.png)

![1566891894094](JavaScript面向对象es6.assets/1566891894094.png)

![1566891914613](JavaScript面向对象es6.assets/1566891914613.png)

+ 方法的查找规则：首先看对象，对象身上是否有相应的方法，如果有就执行这个对象上的sing

+ 如果没有相应的方法，因为有_proto_的存在，就去构造函数原型对象prototype身上去查找方法

![1566892160688](JavaScript面向对象es6.assets/1566892160688.png)

![1566892197585](JavaScript面向对象es6.assets/1566892197585.png)

# 构造函数和原型

![1566892478721](JavaScript面向对象es6.assets/1566892478721.png)

![1566892531942](JavaScript面向对象es6.assets/1566892531942.png)

+ 很多情况下，我们需要手动的利用constructor这个属性只会原来的构造函数
+ 

![1566892738921](JavaScript面向对象es6.assets/1566892738921.png)

![1566892841706](JavaScript面向对象es6.assets/1566892841706.png)

![1566892906228](JavaScript面向对象es6.assets/1566892906228.png)

# 构造函数。实例。和原型对象三者之间的关系

![1566893166955](JavaScript面向对象es6.assets/1566893166955.png)

# 原型链

![1566893500550](JavaScript面向对象es6.assets/1566893500550.png)

![1566893549111](JavaScript面向对象es6.assets/1566893549111.png)

![1566893575218](JavaScript面向对象es6.assets/1566893575218.png)

![1566893609459](JavaScript面向对象es6.assets/1566893609459.png)

# JavaScript的成员查找机制

![1566893915476](JavaScript面向对象es6.assets/1566893915476.png)

# 原型对象this指向

+ 1.在构造函数中，里面this指向的是对象实例
+ 2.原型对象函数里面的this指向的是实例对象

# 原型对象的应用

对Array（数组）对象扩展对象方法

![1566894623338](JavaScript面向对象es6.assets/1566894623338.png)

![1566895004754](JavaScript面向对象es6.assets/1566895004754.png)

# 继承

![1566895151082](JavaScript面向对象es6.assets/1566895151082.png)

call（）

![1566895255723](JavaScript面向对象es6.assets/1566895255723.png)

![1566895271465](JavaScript面向对象es6.assets/1566895271465.png)

![1566901808829](JavaScript面向对象es6.assets/1566901808829.png)

# 用原型对象实现继承

![1566903023183](JavaScript面向对象es6.assets/1566903023183.png)

![1566903055042](JavaScript面向对象es6.assets/1566903055042.png)

![1566911228865](JavaScript面向对象es6.assets/1566911228865.png)

# 类的本质

+ 类的本质其实还是一个函数，我们可以简单的认为类就是构造函数的另外一种写法

![1566912012277](JavaScript面向对象es6.assets/1566912012277.png)

![1566912040112](JavaScript面向对象es6.assets/1566912040112.png)

# es5中新增的方法

## 数组方法

![1566912163759](JavaScript面向对象es6.assets/1566912163759.png)

![1566912205784](JavaScript面向对象es6.assets/1566912205784.png)

![1566912256087](JavaScript面向对象es6.assets/1566912256087.png)

![1566912354808](JavaScript面向对象es6.assets/1566912354808.png)

![1566915553467](JavaScript面向对象es6.assets/1566915553467.png)

some（）

![1566954836390](JavaScript面向对象es6.assets/1566954836390.png)

![1566955014942](JavaScript面向对象es6.assets/1566955014942.png)

+  filter也是查找满足条件的元素，返回的是一个数组，而且是把所有满足条件的元素返回回来
+ some也是查找满足条件的元素是否存在，返回的是一个布尔值，如果查找到第一个满足条件的元素就终止循环

##  forEach和some的区别



![1566959704927](JavaScript面向对象es6.assets/1566959704927.png)

![1566959911689](JavaScript面向对象es6.assets/1566959911689.png)

## 字符串方法

trim（）

![1566960018516](JavaScript面向对象es6.assets/1566960018516.png)

## 对象方法

![1566978766310](JavaScript面向对象es6.assets/1566978766310.png)

![1566978794893](JavaScript面向对象es6.assets/1566978794893.png)

![1566979175288](JavaScript面向对象es6.assets/1566979175288.png)

![1566979272242](JavaScript面向对象es6.assets/1566979272242.png)

![1566979638560](JavaScript面向对象es6.assets/1566979638560.png)

![1566981857262](JavaScript面向对象es6.assets/1566981857262.png)

# 函数的定义和调用

+ 函数声明方式function关键字（命名函数）
+ 函数表达式（匿名函数）
+ new Function（）

![1566982961270](JavaScript面向对象es6.assets/1566982961270.png)

![1566983031863](JavaScript面向对象es6.assets/1566983031863.png)

 

![1566983954630](JavaScript面向对象es6.assets/1566983954630.png)

![1566984090388](JavaScript面向对象es6.assets/1566984090388.png)

# 函数内的this的指向

![1566984407354](JavaScript面向对象es6.assets/1566984407354.png)

# call方法

![1566998558620](JavaScript面向对象es6.assets/1566998558620.png)

![1567045950226](JavaScript面向对象es6.assets/1567045950226.png)

![1567046881714](JavaScript面向对象es6.assets/1567046881714.png)

bind()

![1567047734257](JavaScript面向对象es6.assets/1567047734257.png)

![1567052472995](JavaScript面向对象es6.assets/1567052472995.png)

![1567053295758](JavaScript面向对象es6.assets/1567053295758.png)

# call apply bind 总结

![1567064729378](JavaScript面向对象es6.assets/1567064729378.png)

主要应用场景

![1567064764248](JavaScript面向对象es6.assets/1567064764248.png)

# 严格模式

开启严格模式

‘use strict’

![1567064858264](JavaScript面向对象es6.assets/1567064858264.png)

# 严格模式中的变化

![1567068191188](JavaScript面向对象es6.assets/1567068191188.png)

![1567068317929](JavaScript面向对象es6.assets/1567068317929.png)

![1567068431433](JavaScript面向对象es6.assets/1567068431433.png)

![1567068737182](JavaScript面向对象es6.assets/1567068737182.png)

![1567068866187](JavaScript面向对象es6.assets/1567068866187.png)

![1567068880698](JavaScript面向对象es6.assets/1567068880698.png)

![1567068999139](JavaScript面向对象es6.assets/1567068999139.png)

![1567069170644](JavaScript面向对象es6.assets/1567069170644.png)

# 高阶函数

+ 高阶函数是对其他函数操作的函数，他接收函数作为参数或将函数作为返回值输出

![1567069389780](JavaScript面向对象es6.assets/1567069389780.png)

![1567069411420](JavaScript面向对象es6.assets/1567069411420.png)

此时fn就是一个高阶函数

函数也是一种数据类型，同样可以作为参数，传递给一个参数使用。最典型就是作为回调函数

![1567070375238](JavaScript面向对象es6.assets/1567070375238.png)

# 闭包

![1567071166277](JavaScript面向对象es6.assets/1567071166277.png)

![1567071262432](JavaScript面向对象es6.assets/1567071262432.png)

![1567071708578](JavaScript面向对象es6.assets/1567071708578.png)

 # 闭包的作用

![1567072392779](JavaScript面向对象es6.assets/1567072392779.png)

闭包的主要作用：延伸了变量的作用范围

闭包的案列

![1567073470636](JavaScript面向对象es6.assets/1567073470636.png)

![1567073901286](JavaScript面向对象es6.assets/1567073901286.png)

# 闭包的案例

![1567348735844](JavaScript面向对象es6.assets/1567348735844.png)

# 正则表达式

正则表达式（regular Expression是用于 匹配字符串中字符组合中模式，在JavaScript中，正则表达式也是对象

![1567349467899](JavaScript面向对象es6.assets/1567349467899.png)

![1567349505808](JavaScript面向对象es6.assets/1567349505808.png)

![1567349624472](JavaScript面向对象es6.assets/1567349624472.png)

# 边界符

![1567349968393](JavaScript面向对象es6.assets/1567349968393.png)

# 字符类

![1567351206041](JavaScript面向对象es6.assets/1567351206041.png)

![1567351352511](JavaScript面向对象es6.assets/1567351352511.png)

![1567352178626](JavaScript面向对象es6.assets/1567352178626.png)

# 量词符

![1567352247919](JavaScript面向对象es6.assets/1567352247919.png)

# 正则表达式的特殊字符

![1567390249599](JavaScript面向对象es6.assets/1567390249599.png)

# 正则表达式中的替换

replace替换

+ replace（）方法可以实现替换字符串操作，用来替换的参数可以是一个字符串或是一个正则表达式
+ 

![1567392839651](JavaScript面向对象es6.assets/1567392839651.png)

![1567392867887](JavaScript面向对象es6.assets/1567392867887.png) 

![1567392898781](JavaScript面向对象es6.assets/1567392898781.png)

![1567392933378](JavaScript面向对象es6.assets/1567392933378.png)

# es6的新增语法

let

+ es6中新增的用于声明变量的关键字
+ let声明的变量只在所处的块级有效
+ 在一个大括号中使用let关键字声明的变量才具有块级作用域，var关键字是不具备这个特点的 
+ 防止循环变量变成全局变量
+ 

![1567399692441](JavaScript面向对象es6.assets/1567399692441.png)

let的特性

+ 不存在 变量提升
+ 暂时性死区（var 跟let的变量名相同，相互不会影响）

![1567401310085](JavaScript面向对象es6.assets/1567401310085.png)

![1567401332014](JavaScript面向对象es6.assets/1567401332014.png)

![1567401558943](JavaScript面向对象es6.assets/1567401558943.png)

![1567408355753](JavaScript面向对象es6.assets/1567408355753.png)

# const关键字

+ 作用：声明常量，常量就是值（内存地址）不能变化的值
+ 具有块级作用域
+ 

![1567408599960](JavaScript面向对象es6.assets/1567408599960.png)

![1567408710410](JavaScript面向对象es6.assets/1567408710410.png)

![1567408861234](JavaScript面向对象es6.assets/1567408861234.png)

# let const  var 的区别

![1567408964833](JavaScript面向对象es6.assets/1567408964833.png)

# 解构赋值

es6中允许从数组中提取值，按照对应的位置，对变量赋值，对象也可以实现解构

## 数组解构

![1567409308784](JavaScript面向对象es6.assets/1567409308784.png)

![1567409369748](JavaScript面向对象es6.assets/1567409369748.png)

![1567409388620](JavaScript面向对象es6.assets/1567409388620.png)

### 对象解构

![1567409947348](JavaScript面向对象es6.assets/1567409947348.png)

![1567421717690](JavaScript面向对象es6.assets/1567421717690.png)

# 箭头函数

+ 箭头函数是用来 简化函数定义语法的
+ 在箭头函数中，如果函数中只有一句代码并且代码的执行结构就是函数的返回值，函数体大括号可以省略
+ 如果形参只有一个，可以省略小括号 

![1567421852348](JavaScript面向对象es6.assets/1567421852348.png)

![1567421884850](JavaScript面向对象es6.assets/1567421884850.png)

![1567421973587](JavaScript面向对象es6.assets/1567421973587.png)

![1567422108525](JavaScript面向对象es6.assets/1567422108525.png)

![1567486964995](JavaScript面向对象es6.assets/1567486964995.png)

![1567486980945](JavaScript面向对象es6.assets/1567486980945.png)

# 箭头函数的this关键字

+ 箭头函数不绑定this关键字，箭头函数中的this，指向的是函数定义位置的上下文this

![1567487224204](JavaScript面向对象es6.assets/1567487224204.png)

# 剩余参数

![1567487990033](JavaScript面向对象es6.assets/1567487990033.png)

![1567488639535](JavaScript面向对象es6.assets/1567488639535.png)

## 剩余参数和解构配合使用

![1567488718827](JavaScript面向对象es6.assets/1567488718827.png)

可以变成

![1567488771909](JavaScript面向对象es6.assets/1567488771909.png)