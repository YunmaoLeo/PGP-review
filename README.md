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
  - [Java Week4 06](#java-week4-06)
    - [在改写时添加关键字 ``Override``](#在改写时添加关键字-override)
    - [Inner class(private or public)](#inner-classprivate-or-public)
    - [Abstraction 抽象](#abstraction-抽象)
    - [抽象方法](#抽象方法)
  - [Java Week 6 07](#java-week-6-07)
    - [Abstraction -> Interfaces](#abstraction---interfaces)
    - [Interface 接口](#interface-接口)
    - [Interface:](#interface)
    - [Interfaces vs. Abstract Class](#interfaces-vs-abstract-class)
    - [使用接口还是类？](#使用接口还是类)
    - [OO programming - Designing a Class](#oo-programming---designing-a-class)
    - [使用可见性修改器``Visibility Modifiers``](#使用可见性修改器visibility-modifiers)
    - [SOLID](#solid)
  - [Java Week4 08](#java-week4-08)
    - [Abstraction](#abstraction)
    - [super and super()](#super-and-super)
    - [Packages](#packages)
    - [Static import](#static-import)
    - [Polymorphism 多态](#polymorphism-多态)
    - [Generics:](#generics)
    - [使用``@Override``](#使用override)
    - [ArrayList:](#arraylist)
    - [为什么要用Generics](#为什么要用generics)
  - [Java week7 01 Exception Handling](#java-week7-01-exception-handling)
    - [Exception handling ``Try,Catch``](#exception-handling-trycatch)
    - [Other types of exception:](#other-types-of-exception)
    - [Declaring Exceptions using ``throws``](#declaring-exceptions-using-throws)
    - [``try,catch,finally,throw,throws``](#trycatchfinallythrowthrows)
    - [FileReader:](#filereader)
    - [BufferedReader](#bufferedreader)
  - [Java week 10 tues](#java-week-10-tues)
    - [Classes that correspond to primitives](#classes-that-correspond-to-primitives)
    - [int and Integer:](#int-and-integer)
    - [Double and Float](#double-and-float)
    - [Character:](#character)
    - [Math Class](#math-class)
    - [Autoboxing:](#autoboxing)
  - [Java week 10 Wed](#java-week-10-wed)
    - [Data Structures(Collections)](#data-structurescollections)
    - [Array 数组](#array-数组)
    - [Stack and queues](#stack-and-queues)
    - [Linked List:](#linked-list)
    - [Tree](#tree)
    - [Binary search tree:](#binary-search-tree)
    - [Frameworks (框架)](#frameworks-框架)
    - [List Methods](#list-methods)
    - [Multithreading of Linked list:](#multithreading-of-linked-list)
    - [Arraylist](#arraylist-1)
    - [Linked list 在面对变量，对象都是不可改变的时候的效果会更好](#linked-list-在面对变量对象都是不可改变的时候的效果会更好)
  - [Week 12](#week-12)
    - [Strings](#strings)
    - [String pool](#string-pool)
    - [String method:](#string-method)
- [Haskell](#haskell)
  - [Chapter 1](#chapter-1)
    - [What is a Functional Language:](#what-is-a-functional-language)
    - [Historical Backgroud:](#historical-backgroud)
  - [Chapter 2](#chapter-2)
    - [List 的一些操作](#list-的一些操作)
    - [Function application 有更高的优先级：](#function-application-有更高的优先级)
    - [Naming Requirements 命名要求](#naming-requirements-命名要求)
    - [Layout Rule](#layout-rule)
  - [Chapter 3](#chapter-3)
    - [type inference 类型推断 & basic types](#type-inference-类型推断--basic-types)
    - [Function:](#function)
    - [Polymorphic Functions 多态函数](#polymorphic-functions-多态函数)
  - [Chapter 4 Defining Functions](#chapter-4-defining-functions)
    - [Conditional expressions:](#conditional-expressions)
    - [List Patterns](#list-patterns)
    - [Lambda Expressions:](#lambda-expressions)
    - [Operator Sections:](#operator-sections)
  - [Chapter 5 List comprehension](#chapter-5-list-comprehension)
    - [List Comprehensions](#list-comprehensions)
    - [Dependent Generators:](#dependent-generators)
    - [Guards](#guards)
    - [Zip Function](#zip-function)
    - [String Comprehensions:](#string-comprehensions)
  - [Chapter 6 Recursioon](#chapter-6-recursioon)
    - [Recursive Functions](#recursive-functions)
    - [Testing timing in GHCi 打开时间显示](#testing-timing-in-ghci-打开时间显示)
    - [Quicksort:](#quicksort)
  - [Chapter 7 Higher-Order Functions](#chapter-7-higher-order-functions)
    - [Higher Order Function](#higher-order-function)
    - [Other Library Functions:](#other-library-functions)
    - [Currying](#currying)
  - [Chapter 8 Declaring Types and Classes](#chapter-8-declaring-types-and-classes)
    - [Type Delclarations](#type-delclarations)
    - [Data Declarations](#data-declarations)
    - [Arithmetic Expression](#arithmetic-expression)
    - [Binary Trees](#binary-trees)
  - [Chapter 10 Interactive Programming](#chapter-10-interactive-programming)
    - [Haskell interactive program](#haskell-interactive-program)
    - [Basic Actions](#basic-actions)
    - [Sequencing](#sequencing)
    - [Derived Primitives](#derived-primitives)
  - [Chapter 15 Lazy evaluation and infinite lists](#chapter-15-lazy-evaluation-and-infinite-lists)
    - [Introduction of how Haskell expression are evaluated](#introduction-of-how-haskell-expression-are-evaluated)
    - [Reduction Strategies](#reduction-strategies)
    - [Thunks](#thunks)
    - [Lazy Evaluation:](#lazy-evaluation)
    - [Modular Programming](#modular-programming)
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
```java
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
+ 在一个class中的两个方法可以使用同一个名字，如果它们使用的参数声明不一样

### Constructor overloading
```java
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
```java
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
```java
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
+ 静态方法不能使用``this``

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
+ 一个被声明了``final`` 或 ``static`` 的方法不可以被改写
+ ``constructors``构造器不可以被改写


## Java Week4 06

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
    + 像方法一样调用  ``XXX.inner_class``
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


## Java Week 6 07

### Abstraction -> Interfaces
+ 只展示相关的细节，隐藏不重要的内容
+ 允许抽象方法和非抽象方法被``overridden``j

### Interface 接口
+ 在很多情况下，接口和一个抽象类很相似，但是接口是为了制定对象的常见行为``specify common behavior for objects``
+ 比如，使用合适的接口，可以指定对象是
  + ``compareble``可比较的 
  + ``edible``可修改的
  + ``readable``可读的
+ 然后抽象类只是未成熟的骨架，必须要用子类

+ Interface:
  + 只能有抽象方法
  + 成员永远是public的
  + 接口只能继承其他的java接口
  + 只有static和final变量
  + Java8 中也允许使用默认和静态方法了
    + Default:
    ```Java
    default void defaultTest(){
      System.out.println("This is default test");
    }
    ```

    + Static:静态方法有完整的函数定义，所以不可以被overridden或改变
    ```Java
    static void staticTest(){
      System.out.println("This is static test);
    }
    ```

### Interface:
+ 接口是一个``reference type``参数类型，和类相似，是抽象方法的合集，一个类implements一个接口，因此继承了接口的抽象方法
+ 同样可以包含``final values, default methods, static methods and inner classes``
 
```Java
public interface MoveableI{
  void move();
}

public class VehicleI implements MoveableI{
  public void move(){
    System.out.println('moves')'
  }
  }
```

+ 定义一个接口
```java
public interface InterfaceName{
  constant declarations;
  abstract method signatures;
  default methods;
  static methods;
}
```

+ ```interface extends interface```
  + ``public interface Bicycle extends Vehicle``
  + ``public interface Fish extends Animal, Food``
  + 这允许了一个类由多个父类``one class to have multiple parents``
  + 通过这样做，我们可以使用接口来规避单一继承的限制
  

### Interfaces vs. Abstract Class
+  在接口中，如果需要涵盖数据，就必须是``constant*``，一个抽象类可以有多种类别的数据，接口是更纯粹的抽象
+  所有的类都共享同一个父类``Object class``， 但是接口没有

### 使用接口还是类？
+ 比较强的``IS-A``关系通常使用类，比如``Staff member is a person``,``A cat is an animal``
+ 一个较弱的``IS-A``关系，也叫做``is-kind-of``，表明一个类有某种特殊的性质
  + 比如，所有的Strings都是可比较的，所以String class implements Comparable interface

```java
interface Parent1{
  default void display(){
    System.out.println("I am your mother")}}
interface Parent2{
  default void display(){
    System.out.println("I am your father")}}

class TestMultParents implements Parent1,Parent2{
  public void display(){
    Parent1.super.display();
    Parent2.super.display();}}

public static void main(String args[]){
  TestMultParents d = new TestMultParents();
  d.display();}
```

result:
```
I am your mother
I am your father
```
+ 两个方法都得到了继承，并且会同时使用出来

### OO programming - Designing a Class
+ Coherence连贯性:
  + 一个类应该描述一个单独的实体，所有的类操作都应该支持一个``coherent purpose``连贯的目的
  + 一个有太多职责的个体可以区分成不同的类来拆分职责

### 使用可见性修改器``Visibility Modifiers``
+ 一个类如果需要隐藏他的数据避免被用户直接访问，就需要使用``private``
+ 一个类也应该隐藏那些不面向使用者的方法

### SOLID
+ Single Responsibility Principle:
  + 一个类应该只有一个职责，一个类不应该承载太多
+ Open Closed Principle
  + 一个类应该允许``extension``继承，但不允许``modification``修改
+ Liskov's substitution principle
  + 一个方法应该对每一个子类对象都可以行得通
  + 一个类可以被他的任意一个子类替代
+ Interface Segregation隔离 Principle
  + 使用者不应该被强制implement他们不需要的methods
  + 尽可能地让接口越小越好
+ Dependncy Inversion Principle
  + 抽象类不应该取决于细节，设计的时候不应该考虑细节
  + 类可以改变，但是要遵循父类的界限

## Java Week4 08

### Abstraction
+ Abstract Classes and Interfaces
+ Abstract Classes(0-100% abstraction)
  + abstract and concrete methods
  + abstract keyword
+ interface (100% abstraction)
  + 方法默认是抽象的

### super and super()
```java
class Animal{
  String colour = 'white';}
class Dog extends Animal{
  String colour = 'black';
  void printColour(){
    System.out.println(colour);
    System.out.println(super.color)}}
```

```java
class Animal{
  Animal(){
    System.out.println('animal is created');
    }}

class Dog extends Animal{
  Dog(){
  super();
    System.out.println('dog is created');
    }}
```

### Packages
+ a group of related classes and interfaces
+ organise teams code
+ 控制了获取代码的权限
+ 包内定义的类必须通过包名获取
+ 当没有包被指定的时候，默认使用``the global (default) no-name package``

<br>

+ ``package pkg1.pkg2;`` pkg2 inside a pkg1
+ compile Myclass.java in pkg1.pkg2:``javac -d . Myclass.java``
+ run Myclass: ``java pkg1.pkg2.Myclass``

+ importing pakages:
  + ``pkg1.pkg2.Myclass v = new pkg1.pkg2.Myclass();``
  + 或者也可以
    + ``import pkg.Myclass;``
    + ``import pkg.*;``
      + 这些申明应该紧跟着``pakage statement`` 但是在任何``class definition``前面

### Static import
+ 使用static import可以导入类中的静态成员
+ 这些静态成员可以直接用他们的名字来调用，不需要加class的名字
  + 比如，使用``import static Math.sqrt`` 或者 ``import static Math.*``
  + 就可以直接使用``sqrt()``而不是``Math.sqrt()``

### Polymorphism 多态
+ Polymorphism is the ability of an object to take on many forms
  + ``Compile time polymorphism``
  + ``Runtime polymorphism``
  + ``Parametric polymorphism``
+ Types of polymorphism
  + ``Method overloading``(compile time polmorphism)
    + 有同样名字的参数可以有不同的类型
  + ``Generics in Java`` 泛型(parameric polymorphism)
  + ``subclass Polymorphism`` (runtime polymorphism)
    + `` is-a relationship``

### Generics:
+ 提供更强大的``type checking``
+ ``remove the need for casting``
+ can be used with collections

### 使用``@Override``
+ 允许编译器检查是否有拼写错误或者是错误的参数
+ 让代码更容易被理解


### ArrayList:
```java
java.util.ArrayList list = new java.util.ArrayList();
list.add("Generics")
list.add(5)
```
运行以上代码会有警告，``"java uses unchecked or unsafe operations."``

给上面的代码加上``Generics``
```java
java.util.ArrayList<String> list =
  new java.util.ArrayList<String>();
  list.add("Generics");
  list.add(5);
```
如上代码编译时会出现错误指向``list.add(5)``

### 为什么要用Generics
+ 好处是可以让编译的时候就发现问题，而不是在run time
+ 一个Generic类或方法允许你指定他们可以允许的types
+ ``Generics is the capability to parameterize types``泛型是参数化类型的能力
+ ``Change location of bugs from runtime to compile time``


## Java week7 01 Exception Handling

### Exception handling ``Try,Catch``
```java
try{
  int result = quotient(n1,n2);
  System.out.println(n1 + '/'+ n2 + 'is' + 'result');
  }
catch (ArithmeticException ex){
  System.out.println("Exception:" + " an integer " + " cannot be divided by zero");
}
```

### Other types of exception:
+ ``ArithmeticException``
+ ``InputMismatchException``程序会不停的读入一个输入直到他是正确的
+ ``IndexOutofBoundsException (array index too big/small)``
+ ``IllegalArgumentException (method has been passed an illegal argument)``

处理错误的输入
```java
do{
  try{
    System.our.print("Enter an integer:");
    int number = input.nextInt();
    continueInput = false;}

  catch (InputMismatchExcpetion ex){
    System.out.println("Try again:");
    input.nextLine();}
  }
while(continueInput);
```

### Declaring Exceptions using ``throws``
+ throws 用来声明一个异常
```java
class ThrouwsThrouw{
  void testMethod(int num) throws IOException, ArithmeticException{
    if(num >=42):
      throw new IOException("IOException");
    else:
      throw new ArithmeticException("Arithmetic");
  }
}

class ThrowsMain{
  public static void main(String args[]){
    try{
      ThrowsThrow obj = new ThrowsThrow();
      obj.testMethod(42);
    }
    catch(Exception ex){
      System.out.println(ex);
    }
  }
}
```

### ``try,catch,finally,throw,throws``
+ throw: ``transfer control from try block to catch block``
+ throws:``specifies the exceptions that a method can throw to the caller, doesn't use try or catch itself.``


### FileReader:
+ The data is a stream of characters
+ ``java.io``
```java
import java.io.FileReader
String fileName = "FRtest.txt";
FileReader input = new FileReader(fileName)
try{
  char [] a = new char[2048];
  fileReader.read(a);

  for (char c : a){
    System.out.print(c);
  }
  finally{
    fileReader.close();
  }
}
```
最后要有fileReader.close()来关闭这个阅读

### BufferedReader
+ 使用其他reader来使用character阅读data，效率更高
+ ``Maintains an internal buffer of 8192 characters``
+ Example:
```java
char[] BRchars = new char[120];

try{
  FileReader file = new FileReader("BRtest.txt");
  BufferedReader BR = new BufferedReader(file);
  BR.read(BRchars);
  System.out.println(BRchars);
  BR.close()
}
catch(Exception e){
  e.getStackTrace();
}
```
## Java week 10 tues

### Classes that correspond to primitives
+ Primitives(int,double...) 不是objects
+ They are passed by value to methods
+ Primitives are immutable(不可改变的)
  + 一个local variable是可以改变的，但那实际上是变成了一个新的变量，而不是被改变了值
  + 例如一个int变量＝4，我们将其变为2，this is a change of 100% of tis identity
+ 有时候我们会需要创建primatives的object version
  + ``int``
    + 32bits
    + 无法从字符串值转换来，`cannot be casted to from a string value`
    + cannot be rebased (hex)无法被转换进制
  + ``Integer``
    + Wrapper class 包装类
    + Used in collections or generics
    + 128 bits
    + String -> Integer -> Hex
      + Integer(String)     .toHexString()


### int and Integer:
+ ``int``:
  + Binary representation of an integer
  + 32 bits
  + 无法从字符串强制转换得来
  + 无法被``rebased``进制转换
+ ``Integer``
  + ``Wrapper class``包装类
    + ``Java.lang.Number is superclass of numeric type wrapper``
  + Used in collections or generics
  + 128 bits
  + String -> Integer -> Hex
    + Integer(String).......toHexString()

### Double and Float
+ Extend Number CLass
+ Constructors:
  + ``Float(double d)`` ``Double(doubel d)``
  + ``Float(float f)``
  + ``Float(String s)`` ``Double(String s)``
    + throw excepion if not a number

### Character:
+ to wrap: Character(char c)
+ to return char: char charValue()

### Math Class
+ Contains static methods
+ min(),max(),avg(),sqrt(),round(),abs()

### Autoboxing:
+ ``Wrapper classes -> primitive types without casting``
+ When method is expecting wrapper class* also when assigning a primitive to a wrapper class or cleection framework class.
```java
class Autoboxing1{
  public static void testAB(Integer i){//Method accepter Integer
    System.out.println(i);
  }
  public static void main(String[] args){
    int n = 42;
    testAB(n); 同样是可以通过的，会被自动转换成Integer
  }
}
```



## Java week 10 Wed

### Data Structures(Collections)
+ ``Collections Framework`` provides a hierarchy of ``interfaces and classes`` that provide solutions to managing groups of objects
+ including ways to store collections
+ Generic implementations of common data structures


### Array 数组
+ array is a collection of similar type of elements数组是一系列相似类型元素的集合
+ ``has continuous memory location`` 有一个连续的内存储存空间
+ Fixed length linear lists 固定长度的线性列表
+ Access via index 使用下表进行访问
+ support ``fast random access`` to element
+ Connection between elements is implicit
  + save space, saves time 元素之间的连接是非显性的
+ 一些内置的static methods
  + ```Arrays.binarySearch(myArray,myKey)```
  + ```Arrays.hashCode(myArray)```
  + ```Arrays.sort(myArray)```

### Stack and queues
+ Stack = Last in First out(LIFO)后进先出，最后进出的先出来
  + ``No random access``
  + Push and Pop
+ Queue = First in First out(FIFO) 先进去的也最先出来
  + No random access
+ Prioritised Queues 有线队列
  + Items added or taken off using som priority metric 使用特定的``priority metric``来添加或者删除元素

### Linked List:
+ Elements accessed more flexibly 获取元素更加灵活
+ 添加或移除一个元素是通过重新排列links，而不是改变数据的位置
+ `One link = singly linked list`
+ `Two links = doubly linked list`
+ 从head开始寻找一个元素的复杂度是O(n)
+ 在任何你确定的位置添加一个元素的复杂度是O(1)

### Tree
+ Root is first item
+ Any node with no subtree is a 'leaf'


### Binary search tree:
+ Each node has link to left and right subtree 每一个节点都有左子树或右子树，如果有的话
+ 其中一边的值会更小 ``smaller values one side``

### Frameworks (框架)
+ sets of pre-written code
+ Used as templates
+ IDEs provide some of these framework ability
+ `Predefined classes and functions`
+ Examples:
  + Play: web development, safe I/O, Database access
  + GWT (Google Web Toolkit):
    + Quick UI builds
    + Used for various Google apps
  + Spring


### List Methods
+ .get(int index): returns the element at the specified position in this list
+ .set(int index, E element): replace the element at the specified position

### Multithreading of Linked list:
+ Many threads can be working on one linked list:``compare and swap``
+ can iterate while changing
+ Arrays require much more 'locking' due to the need to change so many elements

### Arraylist
+ support dynamic arrays 支持动态数组
+ Automatically enlarges when needed 在需要的时候自动扩容
+ 3 constructors三个构造器
  + ``ArrayList(0)``  // build empty Arraylist
  + ``ArrayList(int capacity)`` // build ArrayList with a specified initial capacity
    + 如果我们需要写入很多，而且我们有一个对于可能的items的大概的估计，那么添加一个capacity进去会更有效率
  + ``ArrayList(Collection c)``// build with elements from collection c
+ Benefits:
  + ``如果读取的次数比写入的次数多，选择ArrayList更好``
  + 有相当多的写入和完全不知道的尺寸，那么使用LinkedList会更好

### Linked list 在面对变量，对象都是不可改变的时候的效果会更好
+ Linked list 一定要有一个head， a reference to the initial memory location
+ ``Null pointer`` for final member to point to一定要让最后一个指针指向Null

## Week 12
### Strings
+ Strings are an object of ``type String (but not a primitive``
  + 字符串是类型String的对象，不是一个primitive
+ Strings are ``immutable`` 字符串是不可变的

### String pool
+ A storage area in memory where strings are stored(String objects)
+ Identical strings just point to same memory location in string poll
  + **String s1 = "TestString";**
  + **String s3 = "TestString";**
  + 这两个都指向同一个内存空间
+ s2.intern(); //check to see if string exists

### String method:
```java
string.replace('w','y');
string.toUpperCase();
string.length();

startsWith()
toLowerCase()
Substring()
```

# Haskell

## Chapter 1

### What is a Functional Language:
+ Funcional Programming is style of programming in which the basic method of computation is the application of functions to arguments.
+ A functional language is one that supports and encourages the functional style

### Historical Backgroud:
+ Lambda calculus -> Lisp -> ISWIM -> FP -> ML -> Miranda -> 1987 Haskell

## Chapter 2

### List 的一些操作
+ head [1,2,3,4] -> 1
+ tail [1,2,3,4] -> [2,3,4]
+ [1,2,3,4,5] !! 2 -> 3 取下标
+ take 3 [1,2,3,4,5] -> [1,2,3]
+ drop 3 [1,2,3,4,5] -> [4,5]
+ length sum product reverse
+ [1,2,3] ++ [4,5] -> [1,2,3,4,5]

### Function application 有更高的优先级：
+ f a+b -> (f a) + b

+ x `f` y -> f x y 只是语法糖 sytacitic sugar

### Naming Requirements 命名要求
+ 函数和参数名必须以小写字母开头:
  + myFun, fun1, arg_2, x'
+ list arguments列表参数必须要有一个``s suffix``后缀
  + xs, ns, nss

### Layout Rule
+ 每一个定义都应该从同一列开始

## Chapter 3

### type inference 类型推断 & basic types
+ Bool
+ Char: single characters
+ String: string of characters
+ Int: fixed-precision integers
+ Integer: arbitrary-precision integers
+ Float: floating-point numbers

### Function:
+ Functions that take their arguments one at a time are called ``curried functions``

### Polymorphic Functions 多态函数
+ A function is called ``polymorhic`` if its type contains one or more type variables 类型涵盖多个种类的变量
  + length :: [a] -> Int

## Chapter 4 Defining Functions

### Conditional expressions:
```
signum :: Int -> Int
signum n = if n<0 then -1 else
              if n==0 then 0 else 1
```
+ conditional expressions 必须要有一个else branch一次可以避免可能的错误

+ ``Guarded Equations``:
```
abs n | n>=0 =n
      | otherwise = -1
```

+ ``Pattern Matching``
  + Many functions have a particularly clear definition using ``pattern matching`` on their arguments
```
(&&) :: Bool -> Bool -> Bool
True && True = True
_    && _    = False
```

+ Underscore symbol '_' is a ``wildcard`` pattern that matches any argument value
  + 下划线是一个可以匹配所有参数值的通配符
+ Patterns are matched in order, and it may mot repeat variables

### List Patterns
+ 列表时使用一个操作符(:)-> called 'cons', 这个操作符可以把一个元素添加到列表
  + head :: [a] -> a
  + head (x:_) = x
  + tail :: [a] -> [a]
  + tail (_:xs) = xs

### Lambda Expressions:
+ Fcuntions can be constructed withouy naming the functions by using ``lambda expressions``
+ \x → x + x : 此函数返回x+x
+ ``λ``用反斜杠 ``\`` 来替代
+ add x y = x + y
  + means:
  + add = \x -> (\y -> x + y)

### Operator Sections:
+ 1 + 2  -> (+) 1 2 -> (1+) 2 -> (+2) 1

## Chapter 5 List comprehension

### List Comprehensions
+ [x^2 | x <- [1..5]]
+ 改变generators生成器的位置也会改变元素的排列
  + [(x,y) | x <- [1,2,3], y <- [4,5]]
    + [(1,4),(1,5),(2,4),(2,5),(3,4),(3,5)]
  + [(x,y) | y <- [4,5], x <- [1,2,3]]
    + [(1,4),(2,4),(3,4),(1,5),(2,5),(3,5)]
  + 会优先将放在前面的generator的元素先过一遍

### Dependent Generators:
+ 后面的生成器依赖于前面的生成器的变量:
  + [(x,y) | x <- [1..3], y<- [x..3]]
    + [(1,1),(1,2),(1,3),(2,2),(2,3),(3,3)]
+ 使用dependent generators, 我们可以定义一个concatenates function
  + concat :: [[a]] -> [a]
  + concat xss = [x | xs <- xss, x <- xs]

### Guards
+ 列表生成式使用``guards``来限制values
+ [x | x <- [1..10], even x]

### Zip Function
+ map two lists to a list of pairs of their corresponding lements
  + zip :: [a] -> [b] -> [(a,b)]
  + zip ['a','b','c'] [1,2,3,4]
    + [('a',1),('b',2),('c',3)]
+ pairs :: [a] -> [(a,a)]
+ pairs xs = zip xs (tail xs)
  + 上述pair代码中，xs 与 tail xs 进行zip，由于长度不同，所以实际上是前n-1个和后n-1个进行zip

### String Comprehensions:
+ String 本身就是一种特殊的列表，所以任何适用于列表的polymorphic function都适用与列表



## Chapter 6 Recursioon

### Recursive Functions
+ fac 0 = 1
+ fac n = n * fac(n-1)

<br>

+ product :: Num a -> [a] -> a
+ product [] =1
+ product (n:ns) = n * product ns

<br>

+ length :: [a] -> Int
+ length []  = 0
+ length (_:xs) = 1 + length xs

### Testing timing in GHCi 打开时间显示
+ :set s+ command

### Quicksort:
```haskell
qsort :: Ord a -> [a] -> [a]
qsort []      = []
qsort [] (x:xs) = []
  qsort smaller ++ [x] ++ qsort larger
  where
      smaller = [a | a <- xs, a <= x]
      larger = [b | b <- xs, b > x]
```

## Chapter 7 Higher-Order Functions

### Higher Order Function
+ 如果一个函数把一个函数当作参数，或者是当作结果来返回，那么这个函数就被称作``higer-order`` function
+ 用处:
  + 1. ``Common programming idioms`` can be encoded as functions within the language itself
  + 2. ``Domain specific languages`` can be defined as collections of higher-order functions
  + 3. ``Encapsulation using partial function application`` can be used to hide implementation detial
  + 4. ``Algebraic properties`` of higher-order functions can be used to reason about programs

+ Define a `map` function:
  + map f xs = [f x | x <- xs] (use list comprehension)
+ or:
  + map f [] = []
  + map f (x:xs) = f x:map f xs (use recursive)

+ higer-order function ``foldr``:
  + ``sum = foldr (+) 0``
    + sum [] = 0
    + sum (x:xs) = x + sum xs
  + ``product = foldr (*) 1``
    + product [] = 0
    + product (x:xs) = x * product xs
  + or = foldr (||) False
  + ``在foldr可以用于简便实现列表的递归函数，只需要使用 foldr 运算符 初始值的形式即可``
+ define foldr
```haskell
foldr :: (a-> b -> b) -> b -> [a] -> b
foldr f v []  = v
foldr f v (x:xs) = f x (foldr f v xs)
```

+ folder 的优点
  + simpler
  + properties of functions defined using foldr can be proved using algebraic properties of foldr, such as ``fusion融合`` and the ``banana split`` rule
  + Advanced program ``optimisations`` can be simpler if foldr is used in place of explicit recursion

### Other Library Functions:
+ function ``(.)`` returns the composition of two functions as a single function 把两个函数结合在一起
```haskell
odd :: Int -> Bool
odd = not . even
```

+ function ``all`` decides if every element of a list satisfies a given predicate, all 用于判断是否列表中的所有元素都符合给定的样式
```haskell
all :: (a-> Bool) -> [a] -> Bool
all p xs = and [p x | x <- xs]
```
<br>

```haskell
all even [2,4,6,8,10]
```
+ function ``any`` 判断列表中是否至少有一个符合给定的样式

+ funcrtion ``takeWhile`` selects elements from a list while a predicate holds of all the elements
```haskell
takeWhile :: (a-> Bool) -> [a] -> [a]
takeWhile p [] = []
takeWhile p (x:xs)
    | p x     = x : takeWhile p xs
    | otherwise = []
```

```haskell
takeWhile (/= ' ') "abc def"  //"abc"
```
上述代码中的``/= ' '``意思是选取引号中字符前的所有内容

+ function ``dropWhile`` 去除所有符合predicate谓词的值
```haskell
dropWhile (==' ') "   abc"  // "abc"
```

### Currying
+ Curring is the process of transforming a function that takes multiple arguments in a tuple as its argumet, into a function that takes just a single argument and returns another function which accepts further arguments, one by one, that the original function would receive in the rest of that tuple
+ f :: a -> (b->c)
  + is the curred form of 
    + g :: (a,b) -> c
+ 优点：Curried form is usually more convenient because it allows ``partial application``
+ All functions in Haskell take just one argument. so ``f :: a -> b -> c`` is really ``f :: a -> (b -> c)``
+ 比如 div :: int -> int -> int  =====>> div :: int -> (int -> int)
  + curry实际上就是，函数首先获取第一个第一个int，返回了一个可以接收int并返回一个int的函数

+ function ``curry`` takes an uncurried function and consturcts a curried version of this function 
  + curry function会获取一个uncurried function并且构造一个这个函数的curried version
```haskell
curry :: ((a,b) -> c) -> (a-> b -> c)
curry f = \x y -> f (x,y)

addUncurried :: (Int, Int) -> Int
addUncurried :: (x,y) = x + y

> addUncarried (1,2) //3
> curry addUncarried 1 2 //3
> :type curry addUncurried :: Int -> Int -> Int
```
+ 相对应的，也存在``uncurry``,效果与curry相反

## Chapter 8 Declaring Types and Classes

### Type Delclarations

+ ``type String = [Char]``
+ ``type Pos = (Int, Int)``

### Data Declarations
+ ``data Bool = False | True`` 此例中，新类型Bool有两个值False 和True
  + 这其中，他的两个值False 和True被称作``constructors`` for the type Bool
+ Type and constructor names must always begin with an ``upper-case letter``
  + Type 与 constructor的名字必须用大写字母开头

+ constructors in a data declaration can also have parameters:
```haskell
data Shape = Circle Float
            | Rect Float Float
//上述data Shape代码中，Circle & Rect都可以视为是函数

square :: Float -> Shape
square n = Rect n n

area :: Shape -> Float
area (Circle r) = pi * r^2
area (Rect x y ) = x * y
```

+ 同样的data declaration自己也可以拥有参数
```haskell
data Maybe a = Nothing | Just a

safehead :: [a] -> Maybe a
safehead [] = Nothing
safehead xs = Just (head xs)
```

+ Recursive Types of data declarations
```haskell
data Nat = Zero | Succ Nat
```

### Arithmetic Expression
```haskell
data Expr = Val Int
          | Add Expr Expr
          | Mul Expr Expr

Add (Val 1) (Mul (Val 2) (Val 3))
```

### Binary Trees
```haskell
data Tree a = Leaf a
            | Node (Tree a) a (Tree a)

occurs :: Ord a => a -> Tree a -> Bool
occurs x (Leaf y)     = x == y
occurs x (Node l y r) = x == y
                      || occurs x l
                      || occurs x r

flatten :: Tree a -> [a]
flatten :: (Leaaf x)  = [x]
flatten (Node l x r) = flatten l
                        ++ [x]
                        ++ flatten r
```

+ 如果一个数被flatten到一个列表后是有序的，那么这个树是``search tree``

## Chapter 10 Interactive Programming

### Haskell interactive program
+ ``IO a``: return a value of type a
+ ``IO ()``:return no result value, () 是没有元素的元组


### Basic Actions
+ getChar :: IO Char
  + 从键盘读取一个character, echoes it to the screen, 并返回此字符的值
+ putChar :: Char -> IO()
  + putChar c写入一个字符到屏幕中，但不返回任何值
+ return :: a -> IO a
  + simply return the value v, without performing any interaction

### Sequencing
+ 有一些单个操作组成的序列动作可以使用``do``关键字
```haskell
act :: IO (Char,Char)
act = do x <- getChar
          getChar
          y <- getChar
          return (x,y)
```
### Derived Primitives
+ Reading a String from the keyboard:
```haskell
getLine :: IO String
getLine :: do x <- getChar
              if x == '\n' then
                  return []
              else
                  do xs <- getLine
                      return (x:xs)
```

+ Writing a String to the screen
```haskell
putStr :: String -> IO()
putStr []     = return ()
putStr (x:xs) = do putChar x
                   putStr xs
```

## Chapter 15 Lazy evaluation and infinite lists

### Introduction of how Haskell expression are evaluated
+ 1. Avoids doing unnecessary evaluation
+ 2. Allows programs to be more ``modular``模块化的
+ 3. Allows us to program with ``infinite lists``无限列表
+ 以上这些techinique被叫做``lazy evaluation``

### Reduction Strategies
+ 在evaluation的每一个阶段都会有很多可能的subexpressions，这个时候有两种通用的策略进行选择
+ 1. Innermost reduction: an innermost reduction is always reduced. 最外层
+ 2. Outermost reduction: an outermost reduction is always reduced. 最内层

+ 给定以下代码，使用innermost reduction
  + 使用innermost reduction在面对如下有无限内层的代码时，会无限循环
```haskell
loop = tail loop

fst (1,loop)
= fst (1, tail loop)
= fst (1, tail (tail loop))
= .. infinite loop, does not terminate
```

+ 使用outermost reduction
  + outermost reduction 通常会在 innermost reduction 运行失败的情况下给出一个结果
  + 然而，outmost reduction可能会需要更多的运算步骤
```haskell
fst (1, loop)
= 1
```

### Thunks
+ Outmost reduction is ``inefficient`` because (3+4)或其他小运算被重复了很多次
  + 解决方法: ``use sharing``

### Lazy Evaluation:
+ 针对以上问题的new evaluation strategy
  + ``Lazy Evaluation = Outmost reduction + Sharing``
  + Facts
    + Lazy Evaluation 从不需要比innermost reduction更多的步骤
    + Haskell使用的是Lazy Evaluation

### Modular Programming
+ ```take 5 [1..]```
+ control : ``take 5``
+ data : ``[1..]``