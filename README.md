# Java
- [Java](#java)
  - [Lecture 01 Week1](#lecture-01-week1)
    - [Java Compilers and the JVM](#java-compilers-and-the-jvm)
    - [Basic Info](#basic-info)
    - [Java Identifiers](#java-identifiers)
    - [Data types:](#data-types)
  - [Lecture 03 Week 2](#lecture-03-week-2)
    - [Keyword ``this``](#keyword-this)
    - [Fundamentals and terminology](#fundamentals-and-terminology)
    - [Keywords are member dependent](#keywords-are-member-dependent)
    - [Arrays](#arrays)
    - [有标签的 ``break``](#有标签的-break)
    - [Access Modifiers 访问修饰符](#access-modifiers-访问修饰符)
    - [Passing Arguments to Methods](#passing-arguments-to-methods)
    - [Method overloading:](#method-overloading)
    - [Constructor overloading](#constructor-overloading)
    - [Static variables:](#static-variables)
    - [Inner classes:](#inner-classes)
  - [Java Week4 PGP05](#java-week4-pgp05)
    - [Constructors vs methods 构造函数和方法](#constructors-vs-methods-构造函数和方法)
    - [``Static`` keyword：](#static-keyword)
    - [Inheritance继承](#inheritance继承)
    - [Overriding：](#overriding)
  - [Java Week3 06](#java-week3-06)
    - [在改写时添加关键字 ``Override``](#在改写时添加关键字-override)
    - [Inner class(private or public)](#inner-classprivate-or-public)
    - [Abstraction 抽象](#abstraction-抽象)
    - [抽象方法](#抽象方法)
## Lecture 01 Week1

### Java Compilers and the JVM
+ ``Java Compilers``不为了CPU而生成machine code，而是为了``Java Virtual Machine(JVM)``
+ ``JVM machine code(bytecode)`` 通常用每台电脑上的``JVM interpreter program``执行
+ 编译到``Java bytecode``比编译成``machine code``更简单：
  + 只需要考虑一种格式``only one format to target``
  + ``JVM is a much simpler machine`` JVM 是一种更简单的机器
  + 相比于真实CPU，对程序来说更convenient
  + 但是没有优化 ``No optimization`` （这一任务被留给了`JIT(Just In Time) compiler`)
  + ``no real middle end``

### Basic Info
+ ``public``: 我们可以从这个``class``外部调用这个方法
+ ``static``: 当JVM对``main``方法进行呼叫时没有对象存在，所以需要有一个``static``method 来允许``invocation from class``调用类
+ ``main``: main 方法必须是static的
+ ``String args[] or String [] args``: 主函数方法可以接收一个``String``，这个String是运行程序时接收的

### Java Identifiers
+ 方法，变量的名字
+ $ _ 英文字母和数字都可以用来组成identifier
+ 第一位字符不可以是数字
+ 大小写区分
+ 避免使用关键字：abstract continue for new switch assert default goto package synchronized boolean do if private this break double implements protected throw byte else import public throws case enum instanceof return transient catch extends int short try char final interface static void class finally long strictfp volatile const float native super while

### Data types:
+ ``byte,short,int,long``
  + ``8,16,32,64位的signed two's complement number``
  + Long型需要有后缀L  ``long a = 999999999999L``
+ float,double
  + ``32,64位的浮点数``
  + 需要后缀f ``float a = 2.2f``
  + 如果``precision required``有精度要求，要使用``integers or BigDecimal``
+ ``boolean``
  + true/false
+ ``char``
  + 16位的``Unicode character``

## Lecture 03 Week 2

### Keyword ``this``
+ ``this`` is a ``implicit argument`` 指代这个函数调用的对象

### Fundamentals and terminology
+ 所有的对象都有一个``state(Fields)``和``behavior(Methods)``
+ Language basics:
  + 变量：
    + Instance variables(non-static fields)
      + 一个类里面的变量，并且在任何方法的外面
      + 当类被实例化的时候就会被初始化的变量
      + Values unique to each instance of a class but differ between instantiations
    + Class Variables(static fields)
      + 一个类里面的变量，并且在任何方法的外面
      + 当类被实例化的时候就会被初始化的变量
      + Static keyword - only one copy of this
    + Local variables
      + 定义在``methods,constructors or blocks``内的变量
      + 退出程序后会被摧毁 ``Destroyed when we exit the method``


### Keywords are member dependent
+ ``Static variables``: 就像是``global variable``
+ 使用static关键字定义的变量。static可以修饰变量和方法，也有static静态代码块。被static修饰的成员变量和成员方法独立于该类的任何对象。也就是说，它不依赖类特定的实例，被类的所有实例共享。只要这个类被加载，Java虚拟机就能根据类名在运行时数据区的方法区内定找到他们。因此，static对象可以在它的任何对象创建之前访问，无需引用任何对象
+ 用public修饰的static成员变量和成员方法本质是全局变量和全局方法，当声明它的类的对象时，不生成static变量的副本，而是类的所有实例共享同一个static变量

+ ``Static Methods``:一个静态方法只能调用其他的静态方法，只能获取静态数据
+ ``Static class``: 最外层的class不能被设置为静态的，而最内层的可以使用static

### Arrays
+ 声明数组：
  + byte[] firstArrayBytes;
  + int[] firstArrayInts;
  + String[] firstArrayStrings;
+ 分配空间：
  + ``firstArrayInts = new int[3]``
  + or ``int [] firstArrayInts = new int[3];``
+ 填充数组
  + ``int [] firstArrayInts = new int[] {9,1,1};``
+ 多维数组
  + ```int [][] grid={ {1,2},{10,20} };```

### 有标签的 ``break``
```
class LabelledLoop {
           public static void main(String args[])
           {
int i,j;
loop1: for(i=1;i<=10;i++) {
                   for(j=1;j<=10;j++)  //second loop
                   {
} }
} }
System.out.print(j + " "); if(j==5)
break loop1;
//Statement 1
```
+ 有标签的break会跳转回到label处


### Access Modifiers 访问修饰符
+ 决定了其他的类是否能使用这个类里面的``field`` or ``invoke a method``
+ Top level:
  + ``public``: 可以被所有的classes使用和看到
  + 没有``access modifier`` 则是``(package-private)`` - package仅有的
+ Member level:
  + ``private``: 只能被自己这个类访问
  + ``protected``: own package and by a subclass of its class in another package (extends)


### Passing Arguments to Methods
+ primitives 和 references 都是通过值来传递的 ``call-by-value``
+ 参数的值是被**复制**进方法的参数的
+ 如果被复制的参数是``主要数据类型primitives``，那么它的改变不会影响到原参数
+ 如果被复制的参数是一个``reference type引用类型``,那么它的改变会影响到对象 ``(String, objects)``

### Method overloading:
+ 在一个class中的两个方法可以使用同一个名字，如果它们泗洪的参数声明不一样

### Constructor overloading
```
class Myclass{
    int x;
    MyClass(){
        x=0;
    }
    MyClass(int i ){
        x=i;
    }
    MyClass(double d){
        x = (int)d;
    }
    MyClass(int i ,int j){
        x = i*j
    }
}
```
在如上代码中，不同的构造函数会基于不同的参数来进行操作
```
MyClass t1 = new MyClass();
MyClass t2 = new MyClass(88);
MyClass t3 = new MyClass(17.23);
MyClass t4 = new MyClass(2,4);
```

### Static variables:
+ 如果声明了一个变量是``static``，那么这个变量会被class的所有实例共享

### Inner classes:
+ 在别的类里面声明的类叫做``inner classes``
+ 它的 ``范围scope`` 是 ``enclosing class``

例子：
```
class Outer {
    int x = 5;
    class Inner {
        void changeX() { x = 3; } // change Outer's x 
    }
    void adjust() {
        Inner inn = new Inner(); 
        inn.changeX(); // Outer's x is now 3
} 
}
```

## Java Week4 PGP05

### Constructors vs methods 构造函数和方法
+ Constructors 构造器：
  + 在对象被创建的时候初始化
  + 当使用new关键词创建对象时，被``隐性调用``
  + 必须``和类的名字是相同的``
  + 构造器不能返回任何东西（因为对象本身就是他要返回的）
+ Methods 方法：
  + 方法在对象已经存在的时候进行操作
  + 方法可以直接地被已存在的对象调用
  + 必须和类的名字不相同
  + 方法必须要被设置有``return something``， 尽管有void

### ``Static`` keyword：
+ ``Variables, Methods, inner Classes``
+ 用来减少JVM的内存使用
+ 让代码更安全（变量通过特殊的方式进行修改）
+ 如果变量是被声明static的，那么在任何对象改变他，适用于所有的对象
+ ``Static methods``在他的对象的类创建之前就可以被调用
+ 静态方法不能是用``this``

### Inheritance继承
+ Class that is inherited is the ``superclass``
+ class that inherits is the ``subclass``
+ 子类会继承父类的所有方法和变量
+ 父类的变化会影响到子类们
+ Subclasses code can change the ‘intention’ of the superclass code
+ 使用关键字``extends``继承
+ ``每个子类只能有一个父类``
+ 一个子类构造器可以调用一个父类的构造器，使用``super()``，但需要在做其他操作之前
+ 如果没有调用父类的构造器，那么会自动调用一个没有参数的构造器
  

### Overriding：
+ 如果一个类从他的父类继承了一个方法，他可以选择``override``掉，除非父类没有标注``final``
+ 如果方法使用相同的名字被重写，在编译时，他们会将原本的方法给替代掉
+ 需要相同的参数和返回类型
+ 一个被声明了``final`` 或 ``or`` 的方法不可以被改写
+ ``constructors``构造器不可以被改写


## Java Week3 06

### 在改写时添加关键字 ``Override``

### Inner class(private or public)
+ 在一个类的里面写类
+ 我们可以将其转变为private
+ 外部类的方法可以初始化内部类
+ 外部类的方法可以被主函数中别的类调用

<br>

+ 可以实现一个别的类都无法获取的类
  + ``static inner class``
    + 静态类可以不初始化就访问
    + 无法获取外部类的实例变量或方法
    + 像方法一样调用  ``XXX.inner_class
  + ``private inner class``
    + 内部类可以获取外部类的私有变量
  + ``Method local inner classes``:
    + 一个内部只有一个方法的类
  + ``Anonymous Inner Class``匿名内部变量：
    + 没有名字的inner class
    + 同时声明和实例化
    + 用于overriding methods

### Abstraction 抽象
+ 隐藏``implementation details`` 并且只展示对象做什么给用户的过程
+ ``Abstract classes and abstract methods``
+ 抽象类不可以被实例化``instantiated``
+ 需要被申明``abstract``
+ ``public abstract class XYZ``
+ 可以是子类
+ 这些继承出去的类被叫做``concrete classes``可继承实体类
+ 一个抽象类是没有用的，除非他被其他类继承了
+ 当每个自己都会override的时候是有用的

### 抽象方法
+ 一个没有任何东西的方法
+ 只有抽象类可以有抽象方法
+ 一个抽象类的子类必须有父类的所有的抽象方法的实现，如果没有，那么仍然是一个抽象类
+ 一个抽象类可以涵盖抽象方法和不抽象方法
+ 如果在一个类里面定义了抽象方法，就必须要把类也定义为抽象的
+ 一个没有抽象方法的类也可以被定义为抽象类

+ Student Code: 20215699
+ Exam Title Duration Dep Date & Time Room
+ COMP1047 Systems and Architecture 2 hrs CS 5/21/2021 14:30 Siyuan Auditorium
+ COMP1039 Programming Paradigms 2 hrs 30 mins CS 5/25/2021 17:00 DB-C05
+ COMP1037 Fundamentals of Artificial Intelligence 1 hr 30 mins CS 5/28/2021 14:00 TB118
+ COMP1035 Software Engineering? 1 hr CS 5/17/2021 17:30 DB-C05