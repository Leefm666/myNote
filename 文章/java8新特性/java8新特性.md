- lambda表达式实质上是一个匿名方法，但该方法并非独立执行，而是实现**函数式接口定义的唯一抽象方法**
- 使用lambda表达式时，会创建实现了函数式的一个匿名类实例
- 可以将lambda表达式视为一个对象，可以将其作为参数传递



# 函数式接口

函数式接口就是有且只有一个抽象方法

## static方法和default方法

函数式接口虽然只有一个抽象方法，但可以有static方法和default方法

### static方法

```java
public interface Interface {
    /**
     * 静态方法
     */
    static void staticMethod() {
        System.out.println("static method");
    }
}
```

**实现接口的类或者子接口不会继承接口中的静态方法**，其他类实现了该接口不会强制实现

### default方法：

```java
public interface Interface {
    /**
     * default方法
     */
    default void print() {
        System.out.println("hello default");
    }
}

```

**注意：如果接口中的默认方法不能满足某个实现类需要，那么实现类可以覆盖默认方法。不用加default关键字，**

# FunctionalInterface注解

**tip 1**: 可以用 **@FunctionalInterface** 标识函数式接口，非强制要求，但有助于编译器及时检查接口是否满足函数式接口定义
 **tip 2**: 在 Java 8 之前，接口的所有方法都是抽象方法，在 Java 8 中新增了接口的默认方法

# lambda表达式

上文提到，lambda 无法独立执行，它必须是实现一个函数式接口的唯一抽象方法。
**每个 lambda 表达式背后必定有一个函数式接口，该表达式实现的是这个函数式接口内部的唯一抽象方法。**

