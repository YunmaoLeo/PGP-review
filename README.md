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


## Java Week 6 07

### Abstraction -> Interfaces
+ 只展示相关的细节，隐藏不重要的内容
+ 允许抽象方法和非抽象方法被``overridden``j

### Interface 接口
+ 在很多情况下，接口和一个抽象类很相似，但是接口是为了制定对象的常见行为``specify common behavior for objects``
+ 比如，使用合适的接口，可以指定对象是
  + ``compareble``可比较的 
  + ``edible``可修改的
  + ``rideable``可读的
+ 然后抽象类只是未成熟的骨架，必须要用子类

+ Interface:
  + 只能有抽象方法
  + 成员永远是public的
  + 借口只能继承其他的java接口
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
+ 接口是一个``reference type``参数类型，和类相似，是抽象方法的合集，一个类implements一个接口，因此继承了借口的抽象方法
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
  + 通过这样做，我们可以使用借口来规避单一继承的限制
  

### Interfaces vs. Abstract Class
+  在借口中，如果需要涵盖数据，就必须是``constant*``，一个抽象类可以有多种类别的数据，借口是更纯粹的抽象
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
  + 无法从字符串强制转换的来
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
  + **String s3 = "TestString:l**
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