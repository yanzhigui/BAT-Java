## JAVA

### 关键字

void byte int long char short float double String StringBuffer StringBuilder Array Collection Collections List ArrayList LinkedList Vector Set HashMap TreeMap LinkedHashMap ConcerrentHashMap Set TreeMap HashMap synchronized volatile transient implements extends public private protected this super static final const null run start thread enmu quicksort mergesort heapsort bubblesort selectsort insertsort stack queue list heap tree avlTree Btree B+Tree RTree throw throws try catch finally break continue instanceof

### java基础

#### 概念

- 面向对象的三大基本特征、
>三大特性是：封装,继承,多态  
>
>所谓封装，也就是把客观事物封装成抽象的类，并且类可以把自己的数据和方法只让可信的类或者对象操作，对不可信的进行信息隐藏。封装是面向对象的特征之一，是对象和类概念的主要特性。 简单的说，一个类就是一个封装了数据以及操作这些数据的代码的逻辑实体。在一个对象内部，某些代码或某些数据可以是私有的，不能被外界访问。通过这种方式，对象对内部数据提供了不同级别的保护，以防止程序中无关的部分意外的改变或错误的使用了对象的私有部分。
>
>
>所谓继承是指可以让某个类型的对象获得另一个类型的对象的属性的方法。它支持按级分类的概念。继承是指这样一种能力：它可以使用现有类的所有功能，并在无需重新编写原来的类的情况下对这些功能进行扩展。 通过继承创建的新类称为“子类”或“派生类”，被继承的类称为“基类”、“父类”或“超类”。继承的过程，就是从一般到特殊的过程。要实现继承，可以通过“继承”（Inheritance）和“组合”（Composition）来实现。继承概念的实现方式有二类：实现继承与接口继承。实现继承是指直接使用基类的属性和方法而无需额外编码的能力；接口继承是指仅使用属性和方法的名称、但是子类必须提供实现的能力；
>
> 
>
>所谓多态就是指一个类实例的相同方法在不同情形有不同表现形式。多态机制使具有不同内部结构的对象可以共享相同的外部接口。这意味着，虽然针对不同对象的具体操作不同，但通过一个公共的类，它们（那些操作）可以通过相同的方式予以调用。
>
>
>五大基本原则 
>单一职责原则SRP(Single Responsibility Principle)
>是指一个类的功能要单一，不能包罗万象。如同一个人一样，分配的工作不能太多，否则一天到晚虽然忙忙碌碌的，但效率却高不起来。
>
>开放封闭原则OCP(Open－Close Principle) 
>一个模块在扩展性方面应该是开放的而在更改性方面应该是封闭的。比如：一个网络模块，原来只服务端功能，而现在要加入客户端功能，
>那么应当在不用修改服务端功能代码的前提下，就能够增加客户端功能的实现代码，这要求在设计之初，就应当将服务端和客户端分开，公共部分抽象出来。
>
>替换原则(the Liskov Substitution Principle LSP) 
>子类应当可以替换父类并出现在父类能够出现的任何地方。比如：公司搞年度晚会，所有员工可以参加抽奖，那么不管是老员工还是新员工，
>也不管是总部员工还是外派员工，都应当可以参加抽奖，否则这公司就不和谐了。
>
>依赖原则(the Dependency Inversion Principle DIP) 具体依赖抽象，上层依赖下层。假设B是较A低的模块，但B需要使用到A的功能，
>这个时候，B不应当直接使用A中的具体类： 而应当由B定义一抽象接口，并由A来实现这个抽象接口，B只使用这个抽象接口：这样就达到
>了依赖倒置的目的，B也解除了对A的依赖，反过来是A依赖于B定义的抽象接口。通过上层模块难以避免依赖下层模块，假如B也直接依赖A的实现，那么就可能造成循环依赖。一个常见的问题就是编译A模块时需要直接包含到B模块的cpp文件，而编译B时同样要直接包含到A的cpp文件。
>
>接口分离原则(the Interface Segregation Principle ISP) 
>模块间要通过抽象接口隔离开，而不是通过具体的类强耦合起来
>
- 面向过程、面向对象、基于对象和继承、派生、多态：http://www.i3geek.com/archives/580
- 编程思想，幻数：http://www.i3geek.com/archives/622

#### 集合类：

- JAVA高级——集合类 http://www.i3geek.com/archives/616
- 详细阐述集合类   http://www.i3geek.com/archives/1233
- HashMap实现原理,源码阅读 http://www.i3geek.com/archives/1262
- HashMap中Key的约束
- HashMap与HashTable的区别
- HashMap与HashSet的关系:http://www.importnew.com/6931.html hashSet是由hashmap实现的
- HashSet的原理：http://www.importnew.com/19208.html
- ArrayList的用法
- List、Set和Map的继承关系
- Collection 和 Collections的区别
- 其他集合类

#### 继承和接口

- interface和abstrat class抽象类的意义与区别:http://www.i3geek.com/archives/1230
- 实现接口，继承类的规则（单继承多实现）
- 接口继承接口
- 继承多个抽象类？
- Overload和Override的区别。Overloaded的方法是否可以改变返回值的类型?
- 对String类的继承
- abstract的method是否可同时是static,是否可同时是native，是否可同时是synchronized
- 构造器Constructor是否可被override?

#### 异常处理

- Error、Exception和RuntimeException的区别，作用又是什么？列举3个以上的RuntimeException
- Java中的异常处理机制的简单原理和应用
- 内存溢出和内存泄露

#### 管道流

- inputStream和outputStream
- reader和inputstream
- Input/OutputStream和Reader/Writer有的区别
- 理解字符和字节
- 一层层的流结构学会字符流和字节流的转换

#### 线程

- 线程的生命周期：http://www.i3geek.com/archives/859
- java线程池：http://www.i3geek.com/archives/823
- 对run和start方法的理解
- 线程同步的基本方法
- 死锁的问题

#### 其他

- 四种引用，强引用、软引用、弱引用和虚引用 ：http://www.i3geek.com/archives/1239
- String与StringBuilder,StringBuffer的区别
- StringBuffer的实现方式，容量扩充
- 对于 String str ="1"+"2"; 产生了几个对象
- equal与==的区别
- hashCode的作用
- 为什么重写equals就必须重写hashCode
- 自动拆装箱：http://www.i3geek.com/archives/990
- NIO
- java动态代理
- 序列化与反序列化
- public、protected、private以及默认的作用域
- Object类的学习和理解，基本的方法
- char类型的大小，对汉字的存储
- java中传值和传引用的理解，四种引用
- 正则表达式

### Java进阶

#### 多线程

- 多线程要注意什么？
- volatile的关键字学习
- 多线程保证同步的所有方法，除了synchronized外还有什么？
- java中sleep和wait的区别：http://www.i3geek.com/archives/1173
- 理解和使用wait/notify
- 如何保证线程的同步和并发
- 守护线程的含义
- 正确的停止一个线程
- 对synchronized的理解，锁的是什么？锁静态方法和非静态方法的区别

#### 虚拟机

##### 内存结构

- 虚拟机的内存结构，堆内存、栈内存、方法区、常量池等：http://www.i3geek.com/archives/1201
- JVM中的内存设置和分配：http://www.i3geek.com/archives/1138
- 分别存储什么，对象和基本成员变量的存储区域

##### GC垃圾回收

`http://www.i3geek.com/archives/1220`

- gc的概念，什么需要回收？
- 怎么判断被回收？有哪些方法
- 引用计数方法，对象引用遍历和分代回收方法是什么
- 怎么避免对象循环引用的回收
- Java中的内存溢出是如何造成的：http://www.i3geek.com/archives/1241
- Java中的内存溢出和C＋＋中的内存溢出，是一个概念吗？：http://www.i3geek.com/archives/1241

##### CLASSLOADER

- 什么是类加载器
- 哪三层类加载器
- 什么加载顺序
- 功能是什么？工作模式是什么？
- 项目中的例子，加载必要jar包
- 反射的原理，什么是反射？
- 反射的运用，反射是否可以调用私有方法

#### 其他

- NIO是什么
- PRC远程服务原理及作用：http://www.i3geek.com/archives/941
- JMS消息服务框架
- io和nio的本质以及使用场景
- java 8的新特性
- hashcode 有哪些算法
- 泛型的实现机制
- Socket编程通常出现的异常有哪些，什么情况下会出现
- 了解JVM启动参数 -verbose -Xms -Xmx的意思

### J2EE

#### 基本概念

- 分清javaEE、Tomcat、JVM等概念：http://www.i3geek.com/archives/848

#### Servlet

- servlet的基本概念
- servlet的生命周期
- servlet中定制session的过期时间
- Servlet中的session工作原理 （禁用cookie如何使用session）
- filter和listener是什么？有什么区别？servlet、filter、listener：http://www.i3geek.com/archives/870
- JSP和Servlet的区别、共同点（JSP的工作原理）。

#### Web框架

- MVC模型概念
- Spring如何实现AOP和IOC的？- 
- Spring IoC 中的BeanFactory：http://www.i3geek.com/archives/878
- Spring AOP 原理：http://www.i3geek.com/archives/912
- Spring的事务管理 ，Spring bean注入的几种方式

# java面试(一线企业校招、社招)
>友情提示：下面面试题和技术难度，主要正对国内一线企业校招和社招，请量力而为，不要信心受挫。
>故，做为致力于一线企业校招的你来说，能把每个知识模块的一小部分问题去深入学习和总结，已经很棒了，加入BAT企业“随心所欲”！

## 基础   

Arrays.sort实现原理和Collection实现原理   
foreach和while的区别(编译之后)   
线程池的种类，区别和使用场景   
分析线程池的实现原理和线程的调度过程   
线程池如何调优   
线程池的最大线程数目根据什么确定   
动态代理的几种方式   
HashMap的并发问题   
了解LinkedHashMap的应用吗  
反射的原理，反射创建类实例的三种方式是什么？   
cloneable接口实现原理，浅拷贝or深拷贝   
Java NIO使用   
hashtable和hashmap的区别及实现原理，hashmap会问到数组索引，hash碰撞怎么解决   
arraylist和linkedlist区别及实现原理   
反射中，Class.forName和ClassLoader区别   
String，Stringbuffer，StringBuilder的区别？   
有没有可能2个不相等的对象有相同的hashcode   
简述NIO的最佳实践，比如netty，mina   
TreeMap的实现原理   

### JVM相关   

类的实例化顺序，比如父类静态数据，构造函数，字段，子类静态数据，构造函数，字段，他们的执行顺序   
JVM内存分代   
Java 8的内存分代改进   
JVM垃圾回收机制，何时触发MinorGC等操作   
jvm中一次完整的GC流程（从ygc到fgc）是怎样的，重点讲讲对象如何晋升到老年代，几种主要的jvm参数等   
你知道哪几种垃圾收集器，各自的优缺点，重点讲下cms，g1   
新生代和老生代的内存回收策略   
Eden和Survivor的比例分配等   
深入分析了Classloader，双亲委派机制   
JVM的编译优化   
对Java内存模型的理解，以及其在并发中的应用   
指令重排序，内存栅栏等   
OOM错误，stackoverflow错误，permgen space错误   
JVM常用参数   
tomcat结构，类加载器流程   
volatile的语义，它修饰的变量一定线程安全吗    
g1和cms区别,吞吐量优先和响应优先的垃圾收集器选择    
说一说你对环境变量classpath的理解？如果一个类不在classpath下，为什么会抛出ClassNotFoundException异常，如果在不改变这个类路径的前期下，怎样才能正确加载这个类？   
说一下强引用、软引用、弱引用、虚引用以及他们之间和gc的关系      

### JUC/并发相关   

ThreadLocal用过么，原理是什么，用的时候要注意什么   
Synchronized和Lock的区别   
synchronized 的原理，什么是自旋锁，偏向锁，轻量级锁，什么叫可重入锁，什么叫公平锁和非公平锁   
concurrenthashmap具体实现及其原理，jdk8下的改版   
用过哪些原子类，他们的参数以及原理是什么   
cas是什么，他会产生什么问题（ABA问题的解决，如加入修改次数、版本号）   
如果让你实现一个并发安全的链表，你会怎么做   
简述ConcurrentLinkedQueue和LinkedBlockingQueue的用处和不同之处   
简述AQS的实现原理    
countdowlatch和cyclicbarrier的用法，以及相互之间的差别?   
concurrent包中使用过哪些类？分别说说使用在什么场景？为什么要使用？  
LockSupport工具   
Condition接口及其实现原理   
Fork/Join框架的理解   
jdk8的parallelStream的理解   
分段锁的原理,锁力度减小的思考    

## Spring   

Spring AOP与IOC的实现原理   
Spring的beanFactory和factoryBean的区别   
为什么CGlib方式可以对接口实现代理？   
RMI与代理模式   
Spring的事务隔离级别，实现原理   
对Spring的理解，非单例注入的原理？它的生命周期？循环注入的原理，aop的实现原理，说说aop中的几个术语，它们是怎么相互工作的？  
Mybatis的底层实现原理      
MVC框架原理，他们都是怎么做url路由的   
spring boot特性，优势，适用场景等   
quartz和timer对比   
spring的controller是单例还是多例，怎么保证并发的安全   

## 分布式相关    

Dubbo的底层实现原理和机制   
描述一个服务从发布到被消费的详细过程   
分布式系统怎么做服务治理   
接口的幂等性的概念   
消息中间件如何解决消息丢失问题    
Dubbo的服务请求失败怎么处理   
重连机制会不会造成错误   
对分布式事务的理解   
如何实现负载均衡，有哪些算法可以实现？  
Zookeeper的用途，选举的原理是什么？      
数据的垂直拆分水平拆分。  
zookeeper原理和适用场景   
zookeeper watch机制   
redis/zk节点宕机如何处理    
分布式集群下如何做到唯一序列号   
如何做一个分布式锁   
用过哪些MQ，怎么用的，和其他mq比较有什么优缺点，MQ的连接是线程安全的吗   
MQ系统的数据如何保证不丢失   
列举出你能想到的数据库分库分表策略；分库分表后，如何解决全表查询的问题。   

## 算法&数据结构&设计模式   

海量url去重类问题（布隆过滤器）  
数组和链表数据结构描述，各自的时间复杂度   
二叉树遍历   
快速排序   
BTree相关的操作    
在工作中遇到过哪些设计模式，是如何应用的   
hash算法的有哪几种，优缺点，使用场景   
什么是一致性hash   
paxos算法   
在装饰器模式和代理模式之间，你如何抉择，请结合自身实际情况聊聊   
代码重构的步骤和原因，如果理解重构到模式？   

## 数据库   

MySQL InnoDB存储的文件结构   
索引树是如何维护的？   
数据库自增主键可能的问题  
MySQL的几种优化   
mysql索引为什么使用B+树   
数据库锁表的相关处理   
索引失效场景    
高并发下如何做到安全的修改同一行数据，乐观锁和悲观锁是什么，INNODB的行级锁有哪2种，解释其含义     
数据库会死锁吗，举一个死锁的例子，mysql怎么解决死锁     

## Redis&缓存相关   

Redis的并发竞争问题如何解决了解Redis事务的CAS操作吗   
缓存机器增删如何对系统影响最小，一致性哈希的实现   
Redis持久化的几种方式，优缺点是什么，怎么实现的   
Redis的缓存失效策略    
缓存穿透的解决办法   
redis集群，高可用，原理     
mySQL里有2000w数据，redis中只存20w的数据，如何保证redis中的数据都是热点数据   
用Redis和任意语言实现一段恶意登录保护的代码，限制1小时内每用户Id最多只能登录5次   
redis的数据淘汰策略   

## 网络相关   

http1.0和http1.1有什么区别   
TCP/IP协议   
TCP三次握手和四次挥手的流程，为什么断开连接要4次,如果握手只有两次，会出现什么   
TIME_WAIT和CLOSE_WAIT的区别   
说说你知道的几种HTTP响应码   
当你用浏览器打开一个链接的时候，计算机做了哪些工作步骤   
TCP/IP如何保证可靠性，数据包有哪些数据组成    
长连接与短连接     
Http请求get和post的区别以及数据包格式   
简述tcp建立连接3次握手，和断开连接4次握手的过程；关闭连接时，出现TIMEWAIT过多是由什么原因引起，是出现在主动断开方还是被动断开方。    

## 其他  

maven解决依赖冲突,快照版和发行版的区别   
Linux下IO模型有几种，各自的含义是什么  
实际场景问题，海量登录日志如何排序和处理SQL操作，主要是索引和聚合函数的应用   
实际场景问题解决，典型的TOP K问题   
线上bug处理流程   
如何从线上日志发现问题    
linux利用哪些命令，查找哪里出了问题（例如io密集任务，cpu过度）   
场景问题，有一个第三方接口，有很多个线程去调用获取数据，现在规定每秒钟最多有10个线程同时调用它，如何做到。    
用三个线程按顺序循环打印abc三个字母，比如abcabcabc。   
常见的缓存策略有哪些，你们项目中用到了什么缓存系统，如何设计的   
设计一个秒杀系统，30分钟没付款就自动关闭交易（并发会很高）   
请列出你所了解的性能测试工具   
后台系统怎么防止请求重复提交？   
有多个相同的接口，我想客户端同时请求，然后只需要在第一个请求返回结果的时候返回给客户端     
