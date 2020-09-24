java面试题分享

## java基础

### java是什么？
Java是由sun公司开发的一种开源免费的编程语言，现被Oracle收购并维护。主要应用于服务器开发
*****
### Java的构成？
1. JVM：Java虚拟机：加载.Class字节码文件并运行。全称：java virtualmachine。
2. JDK：Java开发工具包，包含jre及编译运行等开发工具。
3. JRE：Java运行环境，包含jvm及运行java程序所需要的类库。
*****
### Java的编译运行过程？（javac与javap的区别）
Javac将.java的文件编译为.class文件，jvm加载class文件并运行。Javap运行.class文件。
*****
### Java的优点？
1. 易学、
2. 强制面向对象、
3. 分布式的：支持internate应用的开发，提供包括（URL、URLConnection、Socket、ServerSocket）
4. 健壮的
5. 安全的、可移植的、动态的。
*****
### Java数据类型（8种）

| 整形     | Byte   | 1B   | 8位  | -128-127       |
| -------- | ------ | ---- | ---- | -------------- |
|          | Short  | 2B   | 16位 | -2^15-(2^15)-1 |
|          | Int    | 4B   | 32位 | -2^31-(2^31)-1 |
|          | Long   | 8B   | 64位 | -2^63-(2^63)-1 |
| 浮点型   | Float  | 4B   | 32位 |                |
|          | Double | 8B   | 64位 |                |
| 字符类型 | Char   | 2B   | 16位 |                |
| 布尔型   | Boolen | 1B   | 8位  | false/true     |

![image-20200924103932972](C:\Users\15715\AppData\Roaming\Typora\typora-user-images\image-20200924103932972.png)
*****
### 数据结构

| 枚举           | Enumeration |
| -------------- | ----------- |
| 位集合         | Bitset      |
| 向量           | Vector      |
| 栈             | Stack       |
| 字典           | Dictionary  |
| 哈希表         | Hashtable   |
| 属性           | Properties  |
| [集合](#_集合) | Collection  |

*******
### 注释

//:单行注释

/**/:多行注释

/***/:文档注释
*****
### Java标识符

1. 命名规则：由字母、数字、下划线、$符号组成。不能以数字开头、大小写敏感、不得使用java中的关键字及保留字。

2. 命名习惯：
>. 包名全部小写，
>. 类的每个词首字母大写。
>. 变量和方法首字母小写，驼峰命名。
>. 常量全部大写，词用_相连。

3.  常见的转义字符：（直接用到字符串当中，是字符串的一部分）
>. “b”退格
>. “f”换页
>. “n”回车
>. “r”换行
>. “t”到下一个tab位置
>. “’”单引号
>. “””双引号
>. “”反斜杠
*****

###  Java关键字

| abstract     | 表明类或者成员方法具有抽象属性                               |
| ------------ | ------------------------------------------------------------ |
| assert       | 断言，用来进行程序调试                                       |
| boolean      | 基本数据类型之一，声明布尔类型的关键字                       |
| break        | 提前跳出一个块                                               |
| byte         | 基本数据类型之一，字节类型                                   |
| case         | 用在switch语句之中，表示其中的一个分支                       |
| catch        | 用在异常处理中，用来捕捉异常                                 |
| char         | 基本数据类型之一，字符类型                                   |
| class        | 声明一个类                                                   |
| const        | 保留关键字，没有具体含义                                     |
| continue     | 回到一个块的开始处                                           |
| default      | 默认，例如，用在switch语句中，表明一个默认的分支。Java8 中也作用于声明接口函数的默认实现 |
| do           | 用在do-while循环结构中                                       |
| double       | 基本数据类型之一，双精度浮点数类型                           |
| else         | 用在条件语句中，表明当条件不成立时的分支                     |
| enum         | 枚举                                                         |
| extends      | 表明一个类型是另一个类型的子类型。对于类，可以是另一个类或者抽象类；对于接口，可以是另一个接口 |
| final        | 用来说明最终属性，表明一个类不能派生出子类，或者成员方法不能被覆盖，或者成员域的值不能被改变，用来定义常量 |
| finally      | 用于处理异常情况，用来声明一个基本肯定会被执行到的语句块     |
| float        | 基本数据类型之一，单精度浮点数类型                           |
| for          | 一种循环结构的引导词                                         |
| goto         | 保留关键字，没有具体含义                                     |
| if           | 条件语句的引导词                                             |
| implements   | 表明一个类实现了给定的接口                                   |
| import       | 表明要访问指定的类或包                                       |
| instanceof   | 用来测试一个对象是否是指定类型的实例对象                     |
| int          | 基本数据类型之一，整数类型                                   |
| interface    | 接口                                                         |
| long         | 基本数据类型之一，长整数类型                                 |
| native       | 用来声明一个方法是由与计算机相关的语言（如C/C++/FORTRAN语言）实现的 |
| new          | 用来创建新实例对象                                           |
| package      | 包                                                           |
| private      | 一种访问控制方式：私用模式                                   |
| protected    | 一种访问控制方式：保护模式                                   |
| public       | 一种访问控制方式：共用模式                                   |
| return       | 从成员方法中返回数据                                         |
| short        | 基本数据类型之一,短整数类型                                  |
| static       | 表明具有静态属性                                             |
| strictfp     | 用来声明FP_strict（单精度或双精度浮点数）表达式遵循[IEEE 754](https://baike.baidu.com/item/IEEE 754)算术规范 |
| super        | 表明当前对象的父类型的引用或者父类型的构造方法               |
| switch       | 分支语句结构的引导词                                         |
| synchronized | 表明一段代码需要同步执行                                     |
| this         | 指向当前实例对象的引用                                       |
| throw        | 抛出一个异常                                                 |
| throws       | 声明在当前定义的成员方法中所有需要抛出的异常                 |
| transient    | 声明不用序列化的成员域                                       |
| try          | 尝试一个可能抛出异常的程序块                                 |
| void         | 声明当前成员方法没有返回值                                   |
| volatile     | 表明两个或者多个变量必须同步地发生变化                       |
| while        | 用在循环结构中                                               |

*****

### Java运算符

>.  算数运算符：
  1.单目运算：+（取正）、-（取负）、++（自增）、--（自减）
	注意：前自增：先自增，后使用；后自增：先使用，后自增。
	前自减：先自减，后使用；后自减：先使用，后自减。
  2.双目运算：+、-、、/、%
  3.三目运算：a>b?true:fasle
*****

>.  关系运算符：
| 等于     | ==   |
| -------- | ---- |
| 不等于   | !=   |
| 大于     | >    |
| 小于     | <    |
| 大于等于 | >=   |
| 小于等于 | <=   |
	注意：==用于比较两个基本数据类型的时候，比较的是两个  变量存储的值是否相等==用于比较两个引用数据类型的时候，比较的是两个引用类型变量所记录的内存地址是否相等
*****

>.  位运算符：（直接操作二进制位）
| &    | 与   |
| ---- | ---- |
| ^    | 或   |
| \|   | 非   |
| ~    | 取反 |
注意：规律：如果操作数A连续异或同一个操作数两次，那么结果还是操作数A
   ```java
class Demo12{
public static void main(String[] args){
	System.out.println(6&3); //结果是:2 
	System.out.println(6|3); //结果是:7
	System.out.println(6^3); //结果是:5
	System.out.println(~7);  // 结果是:-8
}}
   ```

*****
>. 逻辑运算：
| &    | 与             |
| ---- | -------------- |
| &&   | 短路与（强与） |
| ^    | 异或           |
| \|   | 或             |
| \|\| | 短路或（强或） |
| !    | 非             |
	注意：
	&&: 只有两边的布尔表达式同时为true，那么结果才是true；否则为false
	||: 只要两边的布尔表达式有一边为true，结果就为true；如果两边同时都为false，才为false
	^: 只要两边的布尔表达式不一致，结果就为true；如果两边的布尔表达式一致，则为false
	&与&&区别:
		1. 相同点：&&与&的运算结果是一样的。
		2. 不同点：使用&&的时候，如果左边的布尔表达式为false，则不会在运算右边的布尔表达式，从而提高了效率；使用&的时候，即使左边的布尔表达式为false，还是会运算右边的布尔表达式。
	|与||区别：
		1. 相同点：||与|的运算结果是一样的
		2. 不同点：使用||的时候，如果左边的布尔表达式为true，则不会在运算右边的布尔表达式，从而提高了效率；使用|的时候，即使左边的布尔表达式为true，还是会运算右边的布尔表达式。
****

>. 赋值运算符：
| =    | 赋值   |
| ---- | ------ |
| +=   | 加等   |
| -=   | 减等   |
| =    | 乘等   |
| /=   | 除等   |
| %=   | 取余等 |
  ```java
class Demo8 {
public static void main(String[] args) {
    	int i = 10; // 把10赋予给i变量。 
    	i+=2;  // 相当于i = i+2; x	
    	System.out.println("i = "+i);//结果是:i=12
    	byte b1 = 1;
		byte b2 = 2;
		b2+=b1;  //相当于b2 = b2+ b1;b2+=b1在编译的时候，java编译器会进行强制类型转换，不需要我们手动去转换。如果写成		b2=b2+b1,则需要我们手动强制类型转换，变成b2=（byte）b2+b1;
		System.out.println("b2="+ b2);//结果是:b2=3}
}
   ```
******


### 数据排序

#### 数组排序算法：

![image-20200924173334399](C:\Users\15715\AppData\Roaming\Typora\typora-user-images\image-20200924173334399.png)

#### 希尔排序：两两比较插入排序。

#### 冒泡排序：

  ```java
private static void sort(int[] array) throws Exception {
    if (array == null || array.length == 0) {
        throw new Exception("the array is null");
    }
    System.out.println("冒泡排序优化前...");
    int n = array.length;
    for (int i = 0; i < n; i++) {
        for (int j = 0; j < n - i - 1; j++) {
            if (array[j] > array[j + 1]) {
                swap(array, j, j + 1);
            }
        }
        System.out.println("" + Arrays.toString(array));}}
  ```

#### 堆排序：

#### 基数排序：

### 变量（局部变量，实例变量、静态变量）

#### 局部变量：
>不是声明在类体括号内的变量。
  1.必须先赋值，后使用，否则编译出错
  2.作用范围：定义开始到代码块结束。
  3.同一范围不允许两个重名变量存在
******

#### 实例变量：对象的属性

#### 静态变量：变量前加static。

```
Public class Temp{
	Int t;//实例变量
	
	public static void main(String[] args){
	int t =1;//局部变量
	system.out.println(t);
	Temp a = new Temp();//创建实例
	System.out.println(a.t);//通过实例访问实例变量。}}
```



### 类及对象

#### 什么是类，什么是对象？
>. 现实世界中是由很多个对象组成的，对象是独立单一的个体
>. 基于对象的共有属性抽取成类。
>.类是类别，包含所有对象的成员变量即特征属性（变量），也可以包含对象的行为（方法体）
```java
Public class Temp{
    Int I;//属性
    
    Public Temp(int i){}//构造器
    
    Public void act（）{XXXX..}//方法
}
```
*****

### Java修饰符

#### 访问修饰符

![image-20200924143407112](C:\Users\15715\AppData\Roaming\Typora\typora-user-images\image-20200924143407112.png)

#### 非访问修饰符

- static：修饰变量，方法、代码块
>
     - 修饰变量：存在方法区中，只有一份;通过a.t来访问;所有对象共享的数据（图片、音频、视频等）。
     - 修饰方法：存在方法区中，只有一份;通过a.t()来访问;不能直接访问实例成员;方法的操作仅与参数有关与对象无关。
     -  代码块：在类加载期间自动执行，类只被加载一次，静态块也只执行一次;加载/初始化静态资源（图片、音频、视频等）时使用。
*****

- final：修饰类、方法和变量，
>
    - 用final修饰的类不能被继承。
    - 修饰变量为常量不能被修改。
    - 修饰方法不能被继承类重写。
******

- abstract：用来创建抽象类和抽象方法。
	注意：abstract和final不能同时使用。Private和abstract不能同时修饰方法。

- synchronized和volatile，主要用于线程。

### 类分类
#### 内部类
- 成员内部类：作为外部类的一个成员存在，与外部类的属性方法并列。
- 局部内部类：在方法中定义的内部类成为局部内部类。注意：不能有访问修饰符，不是外部类的一部分，可以访问当前代码块内的常量及外部类的所有成员。
- 静态内部类：
>
    - （嵌套类）静态内部类可以用访问修饰符修饰;
    - 可以定义静态或非静态成员;
    - 只能访问外部类的静态成员（静态变量和静态方法）;
    - 不能访问外部类的非静态成员;
    - 外部类访问内部类的静态成员：内部类.静态成员
    - 外部类访问内部类的非静态成员：实例化内部类即可。
*****

- 匿名内部类：即没有名字的内部类。使用内部类的场景：
>
     -  只用到一个类的实例；
     - 类在定义后马上用到
     - 类非常小，给类命名不会导致代码更容易被理解。
	 注意：
     - 匿名内部类中不能有构造方法;
     - 不能定义任何静态成员、方法和类;
     - 不能被访问权限修饰符修饰;
     - 只能创建匿名内部类的一个实例;
     - 一个匿名内部类一定是在new后面，用其隐含实现一个借口或实现一个类;
     - 因匿名内部类为局部内部类，所以局部内部类的所有县乃至都对其有效。
******

#### 内部类注意事项
- 内部类的继承问题
- 内部类的重载问题
- 从多层嵌套类中访问外部
******

### 内存空间的分配及回收

![image-20200924143006910](C:\Users\15715\AppData\Roaming\Typora\typora-user-images\image-20200924143006910.png)

******
#### JVM是java虚拟机，

JVM构成：堆、栈、方法区

- JVM
    - 不同区域存储数据：
        - 栈：局部变量表、动态链接、操作数栈，存储变量地址
        - 堆：常量（jdk1.7之后）、所有对象的实例和数组、编译后的代码（jdk1.7之后）
        - 方法区：类的信息、静态变量、常量、设置参数：启动时分配内存-Xms，最大内存-Xmx

- JMM jvm内存模型
    - Jdk1.7与jdk1.8的区别：jvm内存模型变动，内存模型为新生代、老年代、永久代（1.8之后为元空间）
    - 新生代：主要存放新建的对象。
    - 老年代：主要存放应用程序中生命周期长的对象。
    - 永久代：内存的永久保存区域

- GC垃圾回收机制：
	- GC是什么：自动内存管理和垃圾清扫机制，对JVM中的内存进行标记，并确定哪些内存要回收。
	- Minor GC：当JVM无法为一个新的对象分配空间时会出发，不会影响到永久代。
	- Major GC：回收老年代。
	- Full GC：Full GC 是针对整个新生代、老年代、元空间的全局范围的GC。

- GC Roots：判断对象的存活(路径判断)，在java中可以作为GC Roots的对象包括：
    - 方法区：类静态属性引用的对象。
    - 方法区：常量引用的对象。
    - 虚拟机栈（本地变量表）中引用的对象。
    - 本地方法栈JNI(Native方法)中引用的对象

- 内存泄露和内存溢出辨析
    - 相同与不同：
        - 什么是内存泄露：发生在数据内存共享区域，GC过后某空间（例如10M）回收不了就是内存泄露。
        
        - 什么是内存溢出：JVM内存区域数据存储空间不够
        
        - 如何避免内存泄露：elements[size] = null;

******

### 循环结构

- 常见的3种循环结构（breake、continue关键字）
    - While（布尔表达式）{}
    - Do..while（布尔表达式）{break}
    - For循环
        - For（int I;布尔表达式;更新）{}
        - 增强for循环（for each）：for（声明语句：表达式）{}


******
### 条件语句
- if语句
>
	```JAVA
	if();{}
	if(){} else{}:
	if(布尔表达式 1){
 	//如果布尔表达式 1的值为true执行代码
	}else if(布尔表达式 2){ 
 	//如果布尔表达式 2的值为true执行代码 
	}else if(布尔表达式 3){ 
 	//如果布尔表达式 3的值为true执行代码 
	}else { 
 	//如果以上布尔表达式都不为true执行代码 }
	if(){if(){}else{}}else{}
	```
*****

- Switch case
>     
     - 语法
        ```java
        switch(expression){ 
         	case value : //语句 
         	break; //可选 
         	case value : //语句 
         	break; //可选 
         	//你可以有任意数量的case语句 
         	default : //可选 //语句 }
        ```
    - 规则：
        - switch 变量类型可以是： byte、short、int 或者 char。从 Java SE 7 开始，switch 支持字符串 String 类型了，同时 case 标签必须为字符串常量或字面量
        - switch case 执行时，一定会先进行匹配，匹配成功返回当前 case 的值，再根据是否有 break，判断是否继续输出，或是跳出判断。
        - switch 语句可以包含一个 default 分支，该分支一般是 switch 语句的最后一个分支（可以在任何位置，但建议在最后一个）。default 在没有 case 语句的值和变量值相等的时候执行。default 分支不需要 break 语句。

******

### Number & math类

- Number类：
    - 所有的包装类（Integer、Long、Byte、Double、Float、Short）都是抽象类 Number 的子类。

![image-20200924173218273](C:\Users\15715\AppData\Roaming\Typora\typora-user-images\image-20200924173218273.png)

- Math类：
    - Math 包含了用于执行基本数学运算的属性和方法，如初等指数、对数、平方根和三角函数
    - Math 的方法都被定义为 static 形式，通过 Math 类可以在主函数中直接调用。
    - 实例：
    >
        ```java
      	public class Test { 
      	public static void main (String []args) {
      		System.out.println("90 度的正弦值：" + Math.sin(Math.PI/2));
      		System.out.println("0度的余弦值：" + Math.cos(0));
      		System.out.println("60度的正切值：" + Math.tan(Math.PI/3));
      		System.out.println("1的反正切值： " + Math.atan(1));
      		System.out.println("π/2的角度值：" +	Math.toDegrees(Math.PI/2));
      		System.out.println(Math.PI); } }
        ```
******

- Number & Math 类方法：

| 方法                                                         | 描述                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [xxxValue()](https://www.runoob.com/java/number-xxxvalue.html) | 将 Number 对象转换为xxx数据类型的值并返回。                  |
| [compareTo()](https://www.runoob.com/java/number-compareto.html) | 将number对象与参数比较。                                     |
| [equals()](https://www.runoob.com/java/number-equals.html)   | 判断number对象是否与参数相等。                               |
| [valueOf()](https://www.runoob.com/java/number-valueof.html) | 返回一个 Number 对象指定的内置数据类型                       |
| [toString()](https://www.runoob.com/java/number-tostring.html) | 以字符串形式返回值。                                         |
| [parseInt()](https://www.runoob.com/java/number-parseInt.html) | 将字符串解析为int类型。                                      |
| [abs()](https://www.runoob.com/java/number-abs.html)         | 返回参数的绝对值。                                           |
| [ceil()](https://www.runoob.com/java/number-ceil.html)       | 返回大于等于( >= )给定参数的的最小整数，类型为双精度浮点型。 |
| [floor()](https://www.runoob.com/java/number-floor.html)     | 返回小于等于（<=）给定参数的最大整数 。                      |
| [rint()](https://www.runoob.com/java/number-rint.html)       | 返回与参数最接近的整数。返回类型为double。                   |
| [round()](https://www.runoob.com/java/number-round.html)     | 它表示四舍五入，算法为 Math.floor(x+0.5)，即将原来的数字加上 0.5 后再向下取整，所以，Math.round(11.5) 的结果为12，Math.round(-11.5) 的结果为-11。 |
| [min()](https://www.runoob.com/java/number-min.html)         | 返回两个参数中的最小值。                                     |
| [max()](https://www.runoob.com/java/number-max.html)         | 返回两个参数中的最大值。                                     |
| [exp()](https://www.runoob.com/java/number-exp.html)         | 返回自然数底数e的参数次方。                                  |
| [log()](https://www.runoob.com/java/number-log.html)         | 返回参数的自然数底数的对数值。                               |
| [pow()](https://www.runoob.com/java/number-pow.html)         | 返回第一个参数的第二个参数次方。                             |
| [sqrt()](https://www.runoob.com/java/number-sqrt.html)       | 求参数的算术平方根。                                         |
| [sin()](https://www.runoob.com/java/number-sin.html)         | 求指定double类型参数的正弦值。                               |
| [cos()](https://www.runoob.com/java/number-cos.html)         | 求指定double类型参数的余弦值。                               |
| [tan()](https://www.runoob.com/java/number-tan.html)         | 求指定double类型参数的正切值。                               |
| [asin()](https://www.runoob.com/java/number-asin.html)       | 求指定double类型参数的反正弦值。                             |
| [acos()](https://www.runoob.com/java/number-acos.html)       | 求指定double类型参数的反余弦值。                             |
| [atan()](https://www.runoob.com/java/number-atan.html)       | 求指定double类型参数的反正切值。                             |
| [atan2()](https://www.runoob.com/java/number-atan2.html)     | 将笛卡尔坐标转换为极坐标，并返回极坐标的角度值。             |
| [toDegrees()](https://www.runoob.com/java/number-todegrees.html) | 将参数转化为角度。                                           |
| [toRadians()](https://www.runoob.com/java/number-toradians.html) | 将角度转换为弧度。                                           |
| [random()](https://www.runoob.com/java/number-random.html)   | 返回一个随机数。                                             |

******

### Character类

******
### String类
- String用途
    - 创建和操作字符串
    - 字符串长度：str.length()
    - 连接字符串：string1.contain（string2）
    - String方法：[java.String API](https://www.runoob.com/manual/jdk1.6/java/lang/String.html)

- String源码中构造方法：
```java
1.// String 为参数的构造方法
public String(String original) {
  this.value = original.value;
  this.hash = original.hash;
}

2.// char[] 为参数构造方法
public String(char value[]) {
  this.value = Arrays.copyOf(value, value.length);
}

3.// StringBuffer 为参数的构造方法
public String(StringBuffer buffer) {
  synchronized(buffer) {
    this.value = Arrays.copyOf(buffer.getValue(), buffer.length	());
  }
}

4.// StringBuilder 为参数的构造方法
public String(StringBuilder builder) {
  this.value = Arrays.copyOf(builder.getValue(), builder.length	());
}
```
******

- 其他重要的构造方法：
    - indexOf()：查询字符串首次出现的下标位置
    - lastIndexOf()：查询字符串最后出现的下标位置
    - contains()：查询字符串中是否包含另一个字符串
    - toLowerCase()：把字符串全部转换成小写
    - toUpperCase()：把字符串全部转换成大写
    - length()：查询字符串的长度
    - trim()：去掉字符串首尾空格
    - replace()：替换字符串中的某些字符
    - split()：把字符串分割并返回字符串数组
    - join()：把字符串数组转为字符串
******

- 为什么 String 类型要用 final 修饰？
    - final修饰的好处：
    - 从 String 类的源码我们可以看出 String 是被 final 修饰的不可继承类，源码如下：
    >
         ```java 
    	 public final class String
    	 implements java.io.Serializable, Comparable<String>,CharSequence {   //...... }
         ```
******

- equals 和 ==的区别是什么？
    - ==对于基本类型来说，用于比较“值”是否相等；而对于引用类型来说，是用于比较两个引用地址是否相同。
    - 查看源码可以知道Object类中也有equals方法：
    >
          ```java
		public boolean equals(Object obj) {
    	    return (this == obj);}
		    ```
    
   //String重写了equals方法把他修改成比较两个字符串的值是否相等：
   public boolean equals(Object anObject) {
    	// 对象引用相同直接返回 true
     	if (this == anObject) { 
      		return true;}
        	// 判断需要对比的值是否为 String类型，如果不是则直接返回false
      	if (anObject instanceof String) {
         		String anotherString = (String)anObject;
        		int n = value.length;
            		if (n == anotherString.value.length) {
                		// 把两个字符串都转换为 char 数组对比
                    	char v1[] = value;
                    	char v2[] = anotherString.value;
                    	int i = 0;
                    	// 循环比对两个字符串的每一个字符
                    	while (n-- != 0) {
                    	// 如果其中有一个字符不相等就 true false，否则继续对比
                    		if (v1[i] != v2[i])
                    		return false;
                        	i++;
                    	}
                    return true;
                 }
             }
             return false;
         }
         ```
******

2. Sahib


******

- String 和 StringBuilder、StringBuffer 有什么区别？
    - 用途：对字符串进行修改。
    - StringBuffer与StringBuilder的区别：
        - 执行效率：StringBuilder >StringBuffer >String
        - String类是不可变类，任何对String的改变都会引发新的String对象的生成
        - StringBuffer是可变类,任何对它所指代的字符串的改变都不会产生新的对象,线程安全的。
        - StringBuilder是可变类，线性不安全的，不支持并发操作，不适合多线程中使用，但其在单线程中的性能比StringBuffer高
    - Stringbuffer 方法:
        - 格式化输出：
            - Printf（）
            - System.out.format()
- String 的 intern() 方法有什么含义？

- String 类型在 JVM（Java 虚拟机）中是如何存储的？编译器对 	String 做了哪些优化？

### 日期时间

- Date

    - 调用方法：[java Date API](https://www.runoob.com/java/java-date-time.html)
    - 日期比较：
        -  使用 getTime() 方法获取两个日期（自1970年1月1日经历的毫秒数值），然后比较这两个值。
        -  使用方法 before()，after() 和 equals()。例如，一个月的12号比18号早，则 new Date(99, 2, 12).before(new Date (99, 2, 18)) 返回true。
        -  使用 compareTo() 方法，它是由 Comparable 接口定义的，Date 类实现了这个接口。

- Calender

- 使用 SimpleDateFormat 格式化日期
```java
	public class DateDemo { 
	public static void main(String args[]) { 
	Date dNow = new Date( ); 
	SimpleDateFormat ft = new SimpleDateFormat ("yyyy-MM-dd hh:mm:ss"); 

	System.out.println("当前时间为: " + ft.format(dNow)); } }
```

- 使用printf格式化日期
    - printf 方法可以很轻松地格式化时间和日期。使用两个字母格式，它以 %t 开头并且以下面表格中的一个字母加上%n结尾：
| 转 换 符 | 说  明                      | 示  例                           |
| -------- | --------------------------- | -------------------------------- |
| c        | 包括全部日期和时间信息      | 星期六 十月 27 14:21:20 CST 2007 |
| F        | "年-月-日"格式              | 2007-10-27                       |
| D        | "月/日/年"格式              | 10/27/07                         |
| r        | "HH:MM:SS PM"格式（12时制） | 02:25:51 下午                    |
| T        | "HH:MM:SS"格式（24时制）    | 14:28:16                         |
| R        | "HH:MM"格式（24时制）       | 14:28                            |
******

实例:
```JAVA
public class DateDemo { 
public static void main(String args[]) { 

// 初始化 Date 对象 

Date date = new Date(); 

//c的使用 

System.out.printf("全部日期和时间信息：%tc%n",date); 

//f的使用 

System.out.printf("年-月-日格式：%tF%n",date); 

//d的使用 

System.out.printf("月/日/年格式：%tD%n",date); 

//r的使用 

System.out.printf("HH:MM:SS PM格式（12时制）：%tr%n",date); //t的使用 

System.out.printf("HH:MM:SS格式（24时制）：%tT%n",date); 

//R的使用 

System.out.printf("HH:MM格式（24时制）：%tR",date); } }
```

### 正则表达式
| 字 符       | 说  明                                                       |
| ----------- | ------------------------------------------------------------ |
|             | 将下一字符标记为特殊字符、文本、反向引用或八进制转义符。例如，"n"匹配字符"n"。"n"匹配换行符。序列""匹配""，"("匹配"("。 |
| ^           | 匹配输入字符串开始的位置。如果设置了 RegExp 对象的 Multiline 属性，^ 还会与"n"或"r"之后的位置匹配。 |
| $           | 匹配输入字符串结尾的位置。如果设置了 RegExp 对象的 Multiline 属性，$ 还会与"n"或"r"之前的位置匹配。 |
|             | 零次或多次匹配前面的字符或子表达式。例如，zo 匹配"z"和"zoo"。 等效于 {0,}。 |
| +           | 一次或多次匹配前面的字符或子表达式。例如，"zo+"与"zo"和"zoo"匹配，但与"z"不匹配。+ 等效于 {1,}。 |
| ?           | 零次或一次匹配前面的字符或子表达式。例如，"do(es)?"匹配"do"或"does"中的"do"。? 等效于 {0,1}。 |
| {n}         | n 是非负整数。正好匹配 n 次。例如，"o{2}"与"Bob"中的"o"不匹配，但与"food"中的两个"o"匹配。 |
| {n,}        | n 是非负整数。至少匹配 n 次。例如，"o{2,}"不匹配"Bob"中的"o"，而匹配"foooood"中的所有 o。"o{1,}"等效于"o+"。"o{0,}"等效于"o"。 |
| {n,m}       | m 和 n 是非负整数，其中 n <= m。匹配至少 n 次，至多 m 次。例如，"o{1,3}"匹配"fooooood"中的头三个 o。'o{0,1}' 等效于 'o?'。注意：您不能将空格插入逗号和数字之间。 |
| ?           | 当此字符紧随任何其他限定符（、+、?、{n}、{n,}、{n,m}）之后时，匹配模式是"非贪心的"。"非贪心的"模式匹配搜索到的、尽可能短的字符串，而默认的"贪心的"模式匹配搜索到的、尽可能长的字符串。例如，在字符串"oooo"中，"o+?"只匹配单个"o"，而"o+"匹配所有"o"。 |
| .           | 匹配除"rn"之外的任何单个字符。若要匹配包括"rn"在内的任意字符，请使用诸如"[sS]"之类的模式。 |
| (pattern)   | 匹配 pattern 并捕获该匹配的子表达式。可以使用 $0…$9 属性从结果"匹配"集合中检索捕获的匹配。若要匹配括号字符 ( )，请使用"("或者")"。 |
| (?:pattern) | 匹配 pattern 但不捕获该匹配的子表达式，即它是一个非捕获匹配，不存储供以后使用的匹配。这对于用"or"字符 (\|) 组合模式部件的情况很有用。例如，'industr(?:y\|ies) 是比 'industry\|industries' 更经济的表达式。 |
| (?=pattern) | 执行正向预测先行搜索的子表达式，该表达式匹配处于匹配 pattern 的字符串的起始点的字符串。它是一个非捕获匹配，即不能捕获供以后使用的匹配。例如，'Windows (?=95\|98\|NT\|2000)' 匹配"Windows 2000"中的"Windows"，但不匹配"Windows 3.1"中的"Windows"。预测先行不占用字符，即发生匹配后，下一匹配的搜索紧随上一匹配之后，而不是在组成预测先行的字符后。 |
| (?!pattern) | 执行反向预测先行搜索的子表达式，该表达式匹配不处于匹配 pattern 的字符串的起始点的搜索字符串。它是一个非捕获匹配，即不能捕获供以后使用的匹配。例如，'Windows (?!95\|98\|NT\|2000)' 匹配"Windows 3.1"中的 "Windows"，但不匹配"Windows 2000"中的"Windows"。预测先行不占用字符，即发生匹配后，下一匹配的搜索紧随上一匹配之后，而不是在组成预测先行的字符后。 |
| x\|y        | 匹配 x 或 y。例如，'z\|food' 匹配"z"或"food"。'(z\|f)ood' 匹配"zood"或"food"。 |
| [xyz]       | 字符集。匹配包含的任一字符。例如，"[abc]"匹配"plain"中的"a"。 |
| [^xyz]      | 反向字符集。匹配未包含的任何字符。例如，"[^abc]"匹配"plain"中"p"，"l"，"i"，"n"。 |
| [a-z]       | 字符范围。匹配指定范围内的任何字符。例如，"[a-z]"匹配"a"到"z"范围内的任何小写字母。 |
| [^a-z]      | 反向范围字符。匹配不在指定的范围内的任何字符。例如，"[^a-z]"匹配任何不在"a"到"z"范围内的任何字符。 |
| b           | 匹配一个字边界，即字与空格间的位置。例如，"erb"匹配"never"中的"er"，但不匹配"verb"中的"er"。 |
| B           | 非字边界匹配。"erB"匹配"verb"中的"er"，但不匹配"never"中的"er"。 |
| cx          | 匹配 x 指示的控制字符。例如，cM 匹配 Control-M 或回车符。x 的值必须在 A-Z 或 a-z 之间。如果不是这样，则假定 c 就是"c"字符本身。 |
| d           | 数字字符匹配。等效于 [0-9]。                                 |
| D           | 非数字字符匹配。等效于 [^0-9]。                              |
| f           | 换页符匹配。等效于 x0c 和 cL。                               |
| n           | 换行符匹配。等效于 x0a 和 cJ。                               |
| r           | 匹配一个回车符。等效于 x0d 和 cM。                           |
| s           | 匹配任何空白字符，包括空格、制表符、换页符等。与 [ fnrtv] 等效。 |
| S           | 匹配任何非空白字符。与 [^ fnrtv] 等效。                      |
| t           | 制表符匹配。与 x09 和 cI 等效。                              |
| v           | 垂直制表符匹配。与 x0b 和 cK 等效。                          |
| w           | 匹配任何字类字符，包括下划线。与"[A-Za-z0-9_]"等效。         |
| W           | 与任何非单词字符匹配。与"[^A-Za-z0-9_]"等效。                |
| xn          | 匹配 n，此处的 n 是一个十六进制转义码。十六进制转义码必须正好是两位数长。例如，"x41"匹配"A"。"x041"与"x04"&"1"等效。允许在正则表达式中使用 ASCII 代码。 |
| num         | 匹配 num，此处的 num 是一个正整数。到捕获匹配的反向引用。例如，"(.)1"匹配两个连续的相同字符。 |
| n           | 标识一个八进制转义码或反向引用。如果 n 前面至少有 n 个捕获子表达式，那么 n 是反向引用。否则，如果 n 是八进制数 (0-7)，那么 n是八进制转义码。 |
| nm          | 标识一个八进制转义码或反向引用。如果 nm 前面至少有 nm 个捕获子表达式，那么 nm 是反向引用。如果 nm 前面至少有 n 个捕获，则 n 是反向引用，后面跟有字符 m。如果两种前面的情况都不存在，则 nm 匹配八进制值 nm，其中 n 和 m 是八进制数字 (0-7)。 |
| nml         | 当 n 是八进制数 (0-3)，m 和 l 是八进制数 (0-7) 时，匹配八进制转义码 nml。 |
| un          | 匹配 n，其中 n 是以四位十六进制数表示的 Unicode 字符。例如，u00A9 匹配版权符号 (©)。 |

 

### 方法

#### Scanner

- 特性：java.util.Scanner 是 Java5 的新特征，我们可以通过 Scanner 类来获取用户的输入。

- Demo：
```JAVA
public class ScannerDemo { 

public static void main(String[] args) { 

Scanner scan = new Scanner(System.in); 

// 从键盘接收数据 

// nextLine方式接收字符串 

System.out.println("nextLine方式接收："); 

// 判断是否还有输入 

if (scan.hasNextLine()) { 

String str2 = scan.nextLine(); 

System.out.println("输入的数据为：" + str2); } 

scan.close(); } }
```

- next（）与nextLine（）的区别：
    - next（）：
        - 一定要读取到有效字符后才可以结束输入。
        - 对输入有效字符之前遇到的空白，next() 方法会自动将其去掉。
        - 只有输入有效字符后才将其后面输入的空白作为分隔符或者结束符。
        - next() 不能得到带有空格的字符串

    - nextLine（）：
        - 以Enter为结束符,也就是说 nextLine()方法返回的是输入回车之前的所有字符。
        - 可以获得空白。

### IO/NIO/Stream、File
- 什么是java.io？
    - Java.io 包几乎包含了所有操作输入、输出需要的类。所有这些流类代表了输入源和输出目标。
    - Java.io 包中的流支持很多种格式，比如：基本类型、对象、本地化字符集等等。
    - 一个流可以理解为一个数据的序列。输入流表示从一个源读取数据，输出流表示向一个目标写数据。

- 输入流输出流层级图。

![image-20200924173155057](C:\Users\15715\AppData\Roaming\Typora\typora-user-images\image-20200924173155057.png)

- Io流的作用？

- 读写文件
    - ·FileInputStream（ByteInputStream/DataInputStream）
        -  该流用于从文件读取数据，它的对象可以用关键字 new 来创建。
        -  有多种构造方法可用来创建对象
        -  可以使用字符串类型的文件名来创建一个输入流对象来读取文件：
        >
           ```java
           InputStream f = new FileInputStream("C:/java/hello");
           ```
        - 可以使用一个文件对象来创建一个输入流对象来读取文件。我们首先得使用 File() 方法来创建一个文件对象：
        >
            ```java
            File f = new File("C:/java/hello");
            InputStream out = new FileInputStream(f);
            ```
    
    - ·FileOutputStream（ByteArrayOutpotStream/DataOutputStream）
        -  该留用来创建文件并向文件写入数据。
        -  如果该流在打开文件进行输出前，目标文件不存在，那么该流会创建该文件。
        -  使用字符串类型的文件名来创建一个输出流对象：
        >
		     ```java
		     OutputStream f = new FileOutputStream("C:/java/hello")
		     ```
		
		- 使用一个文件对象来创建一个输出流来写文件。我们首先得使用File()方法来创建一个文件对象：
		>
		     ```java
		     File f = new File("C:/java/hello"); 
		     OutputStream f = new FileOutputStream(f);
		     ```
******

- 文件和IO
    - File Class
    - FileReader Class
    - FileWriter Class

- Java中的目录
    - 创建目录：File类中有两个方法来创建文件夹
        - mkdir():创建一个文件夹，成功则返回
        - mkdirs()
    - 读取目录
    - 删除目录或文件
******

### 异常处理

- Exception类的层次

![image-20200924173142340](C:\Users\15715\AppData\Roaming\Typora\typora-user-images\image-20200924173142340.png)

- Java内置异常类

| 异常                            | 描述                                                         |
| ------------------------------- | ------------------------------------------------------------ |
| ArithmeticException             | 当出现异常的运算条件时，抛出此异常。例如，一个整数"除以零"时，抛出此类的一个实例。 |
| ArrayIndexOutOfBoundsException  | 用非法索引访问数组时抛出的异常。如果索引为负或大于等于数组大小，则该索引为非法索引。 |
| ArrayStoreException             | 试图将错误类型的对象存储到一个对象数组时抛出的异常。         |
| ClassCastException              | 当试图将对象强制转换为不是实例的子类时，抛出该异常。         |
| IllegalArgumentException        | 抛出的异常表明向方法传递了一个不合法或不正确的参数。         |
| IllegalMonitorStateException    | 抛出的异常表明某一线程已经试图等待对象的监视器，或者试图通知其他正在等待对象的监视器而本身没有指定监视器的线程。 |
| IllegalStateException           | 在非法或不适当的时间调用方法时产生的信号。换句话说，即 Java 环境或 Java 应用程序没有处于请求操作所要求的适当状态下。 |
| IllegalThreadStateException     | 线程没有处于请求操作所要求的适当状态时抛出的异常。           |
| IndexOutOfBoundsException       | 指示某排序索引（例如对数组、字符串或向量的排序）超出范围时抛出。 |
| NegativeArraySizeException      | 如果应用程序试图创建大小为负的数组，则抛出该异常。           |
| NullPointerException            | 当应用程序试图在需要对象的地方使用 null 时，抛出该异常       |
| NumberFormatException           | 当应用程序试图将字符串转换成一种数值类型，但该字符串不能转换为适当格式时，抛出该异常。 |
| SecurityException               | 由安全管理器抛出的异常，指示存在安全侵犯。                   |
| StringIndexOutOfBoundsException | 此异常由 String 方法抛出，指示索引或者为负，或者超出字符串的大小。 |
| Java.Lang包中的检查性异常类     |                                                              |
| UnsupportedOperationException   | 当不支持请求的操作时，抛出该异常。                           |
| ClassNotFoundException          | 应用程序试图加载类时，找不到相应的类，抛出该异常。           |
| CloneNotSupportedException      | 当调用 Object 类中的 clone 方法克隆对象，但该对象的类无法实现 Cloneable 接口时，抛出该异常。 |
| IllegalAccessException          | 拒绝访问一个类的时候，抛出该异常。                           |
| InstantiationException          | 当试图使用 Class 类中的 newInstance 方法创建一个类的实例，而指定的类对象因为是一个接口或是一个抽象类而无法实例化时，抛出该异常。 |
| InterruptedException            | 一个线程被另一个线程中断，抛出该异常。                       |
| NoSuchFieldException            | 请求的变量不存在                                             |
| NoSuchMethodException           | 请求的方法不存在                                             |
| ClassNotFoundException          | 应用程序试图加载类时，找不到相应的类，抛出该异常。           |
| CloneNotSupportedException      | 当调用 Object 类中的 clone 方法克隆对象，但该对象的类无法实现 Cloneable 接口时，抛出该异常。 |
| IllegalAccessException          | 拒绝访问一个类的时候，抛出该异常。                           |
| InstantiationException          | 当试图使用 Class 类中的 newInstance 方法创建一个类的实例，而指定的类对象因为是一个接口或是一个抽象类而无法实例化时，抛出该异常。 |
| InterruptedException            | 一个线程被另一个线程中断，抛出该异常。                       |

 

- 异常方法

| 方法                                        | 说明                                                         |
| ------------------------------------------- | ------------------------------------------------------------ |
| public String getMessage()                  | 返回关于发生的异常的详细信息。这个消息在Throwable 类的构造函数中初始化了。 |
| public Throwable getCause()                 | 返回一个Throwable 对象代表异常原因。                         |
| public String toString()                    | 使用getMessage()的结果返回类的串级名字。                     |
| public void printStackTrace()               | 打印toString()结果和栈层次到System.err，即错误输出流。       |
| public StackTraceElement [] getStackTrace() | 返回一个包含堆栈层次的数组。下标为0的元素代表栈顶，最后一个元素代表方法调用堆栈的栈底。 |
| public Throwable fillInStackTrace()         | 用当前的调用栈层次填充Throwable 对象栈层次，添加到栈层次任何先前信息中。 |

 

- 捕捉异常（关键字）

Try{}catch{}finally{}throw、throwable

- 自定义异常
    - 所有异常都必须是 Throwable 的子类。
    - 如果希望写一个检查性异常类，则需要继承 Exception 类。
    - 如果你想写一个运行时异常类，那么需要继承 RuntimeException 类。

- 通用异常
    - JVM(Java虚拟机) 异常：由 JVM 抛出的异常或错误。
      例如：NullPointerException 类，ArrayIndexOutOfBoundsException 类，ClassCastException 类。
    - 程序级异常：由程序或者API程序抛出的异常。
    例如:IllegalArgumentException 类，IllegalStateException 类
******

## 面向对象

### 面向对象的特性

封装、继承、抽象、多态。

- 继承 
    - 说明：
        - 单继承：A extend B
        - 多重继承： A extend B B extend C
        - 不同类继承同一个类：A extend C B extend C
        - 同一个类可以被多个类继承，不能继承多个父类
    - 特性：
        - 子类拥有父类所有非private的属性、方法。
        - 子类可以拥有自己的属性、方法。即子类对父类的扩展。
        - 子类可以用自己的方式
******

- 多态
    - 多态的优点：
        - 消除类之间的耦合关系；
        - 可替换性；
        - 可扩充性；
        - 接口性；
        - 灵活性；
        - 简化性；
    - 多态存在的三个必要条件
        - 继承
        - 重写
        - 父类引用指向子类对象
    - 多态的实现方式
        - 重写
        - 接口
        - 抽象类和抽象方法

- 封装
    - 封装的优点：
        - 良好的封装能减少耦合
        - 类的内部结构可以自由的修改
        - 可以对成员变量进行更精准的控制
        - 隐藏信息，实现细节

    - 封装步骤：
        - 修改属性访问权限（一般为private）
        - 实现属性的对外公共方法的访问（getter、setter）
        - Example：
        >
            ```java
            Public class person{
            	Private String name;
            	Private String age;
            	Private String address;
            	Public String getName(){ return name;}
            	Public String getAge(){ return age;}
            	Public String getAdress(){ return address;}
            	Public void setName(String name){this.name = name;}
            	Public void setAge(String age){this.age = age;}
            	Public void setAdress(String address){
            		this.adress = address;
            	}
            }
            ```
******

- 抽象
    - 抽象类型:抽象类/抽象方法
    
    - 抽象类：
        - Java中抽象类表示一种继承关系，一个类只能继承（extends）一个抽象类，但可以实现（implements）多个接口。
        
    - 抽象方法：
        - 一个类声明了抽象方法，必定是个抽象类；
        - 任何子类必须重写父类的抽象方法，或者声明自身为抽象类
        - 定义接口：Interface
    - 总结：
        - 抽象类直接被实例化会编译失败
        - 抽象类不一定包含抽象方法，但是有抽象方法的类必定是抽象类
        - 抽象类的抽象方法只是声明，没有方法体
        - 构造方法，类方法（用static修饰的方法）不能声明为抽象方法
        - 抽象类的子类必须给出抽象类中的抽象方法的具体实现，除非该子类也是抽象类。

- 包（package）
******

## 集合

### 集合框架
![image-20200924173110452](C:\Users\15715\AppData\Roaming\Typora\typora-user-images\image-20200924173110452.png)

![image-20200924173120731](C:\Users\15715\AppData\Roaming\Typora\typora-user-images\image-20200924173120731.png)

******
### 集合接口
| 接口        | 接口描述                                                     |
| ----------- | ------------------------------------------------------------ |
| Collection  | Collection最基本的集合接口，一个 Collection 代表一组 Object，即 Collection 的元素, Java不提供直接继承自Collection的类，只提供继承于的子接口(如List和set)。Collection 接口存储一组不唯一，无序的对象。 |
| List        | List 接口是一个有序的 Collection，使用此接口能够精确的控制每个元素插入的位置，能够通过索引(元素在List中位置，类似于数组的下标)来访问List中的元素，第一个元素的索引为 0，而且允许有相同的元素。List 接口存储一组不唯一，有序（插入顺序）的对象。 |
| Set         | Set具有与 Collection 完全一样的接口，只是行为上不同，Set 不保存重复的元素。Set 接口存储一组唯一，无序的对象。 |
| SortedSet   | 继承于Set保存有序的集合。                                    |
| Map         | Map 接口存储一组键值对象，提供key（键）到value（值）的映射。 |
| Map.Entry   | 描述在一个Map中的一个元素（键/值对）。是一个Map的内部类。    |
| SortedMap   | 继承于 Map，使 Key 保持在升序排列。                          |
| Enumeration | 这是一个传统的接口和定义的方法，通过它可以枚举（一次获得一个）对象集合中的元素。这个传统接口已被迭代器取代。 |

******

### 集合实现类

| 接口       | 接口描述                                                     |
| ---------- | ------------------------------------------------------------ |
| Vector     | 该类和ArrayList非常相似，但是该类是同步的，可以用在多线程的情况，该类允许设置默认的增长长度，默认扩容方式为原来的2倍。 |
| Stack      | 栈是Vector的一个子类，它实现了一个标准的后进先出的栈。       |
| Dictionary | Dictionary 类是一个抽象类，用来存储键/值对，作用和Map类相似。 |
| Hashtable  | Hashtable 是 Dictionary(字典) 类的子类，位于 java.util 包中。 |
| Properties | Properties 继承于 Hashtable，表示一个持久的属性集，属性列表中每个键及其对应值都是一个字符串。 |
| BitSet     | 一个Bitset类创建一种特殊类型的数组来保存位值。BitSet中数组大小会随需要增加。 |
******

### 迭代器

- 遍历ArrayList
  实例：
```java
import java.util.; 

public class Test{ 

public static void main(String[] args) { 

List<String> list=new ArrayList<String>(); 

list.add("Hello"); 

list.add("World"); 

list.add("HAHAHAHA"); 

//第一种遍历方法使用 For-Each 遍历 List 

for (String str : list) { 

//也可以改写 for(int i=0;i<list.size();i++) 这种形式 

System.out.println(str); 

}	 

//第二种遍历，把链表变为数组相关的内容进行遍历 

String[] strArray=new String[list.size()]; 

list.toArray(strArray); 

for(int i=0;i<strArray.length;i++) 

//这里也可以改写为 for(String str:strArray) 这种形式 { 

System.out.println(strArray[i]); 

} 

//第三种遍历 使用迭代器进行相关遍历 

Iterator<String> ite=list.iterator(); 

while(ite.hasNext())//判断下一个元素之后有值 { 

System.out.println(ite.next()); } } }
```

- 遍历Map
  实例：
```java
public class Test{ 

public static void main(String[] args) { 

Map<String, String> map = new HashMap<String, String>(); 

map.put("1", "value1");

map.put("2", "value2"); 

map.put("3", "value3"); 

//第一种：普遍使用，二次取值 

System.out.println("通过Map.keySet遍历key和value："); 

for (String key : map.keySet()) { 

System.out.println("key="+key+"and value="+map.get(key));} 

//第二种 

System.out.println("通过Map.entrySet使用iterator遍历key和value："); 

Iterator<Map.Entry<String,String>> it = map.entrySet().iterator();

while (it.hasNext()) { 

Map.Entry<String, String> entry = it.next();

System.out.println("key= " + entry.getKey() + " and value= " + entry.getValue()); } 

//第三种：推荐，尤其是容量大时 

System.out.println("通过Map.entrySet遍历key和value"); 

for (Map.Entry<String, String> entry : map.entrySet()) { 

System.out.println("key= " + entry.getKey() + " and value= " + entry.getValue()); } 

//第四种 System.out.println("通过Map.values()遍历所有的value，但不能遍历key"); 

for (String v : map.values()) { 

System.out.println("value= " + v); } } }
```

- 比较器:使用 Java Comparator

## 泛型

1. 什么是泛型？

2. 泛型的作用？

## 序列化

1.  什么是序列化：将对象的状态字节话写入byte流，处理对象流的机制。

2.  序列化有什么作用：解决对象流进行读写操作是发生的问题。

3.  序列化的实现：将需要被序列化的类的实现
    - 将需要被序列化的类实现Serializeable接口
    - 使用一个输出流例如FileOutputStream来构造一个ObjectOutputStream（对象流）对象
    - 使用ObjectOutputStream的writeObject（Object obj）方法就可以将参数为obj的对象写出，要恢复的话则使用输入流。
    注意：
        - 某个类能被序列化，其子类也可以被序列化。
        - 声明为static和transien类型的成员数据不能被序列化，因为static代表类的状态，transient代表对象的临时数据。
        - writeObject和readObject方法本身就是线程安全的，传输过程中不允许被并发访问的。所以对象能一个一个不断的穿过来。

4.什么是线程安全？线程不能并发访问的即线程安全的。

******

## 多线程

### 进程与线程的区别

- 进程：指一个内存中运行的应用程序，每个进程都有一个独立的内存空间，一个应用程序可以同时运行多个进程;进程也是应用程序的一次执行过程，是系统运行程序的基本单元;系统运行一个程序就是一个进程从创建运行至消亡的过程。

- 线程：线程是进程内部的一个执行单元;一个进程可以同时并发运行多个线程，可以理解为一个进程相当于单个CPU操作系统，线程是系统中运行的多个任务。

- 区别：

    - 进程：进程拥有独立的内存空间，进程中的数据存放（堆栈空间）是独立的，至少有一个线程。

    - 线程：堆空间共享栈空间独立，线程消耗资源比进程小。

    - Notice：Java中程序的进程里面至少包含两个线程，其中一个是main()方法主线程，另一个是GC垃圾回收机制线程。每当使用Java命令执行一个类时，启动一个JVM，每一个JVM实际上就是在操作系统中启动一个线程，Java本身具备了垃圾回收机制，所以Java运行时至少启动两个线程。因为一个线程耗费的资源比另起一个进程小的多，所以在多任务开发时优先考虑多线程。进程中的多个线程是并发运行的微观上又先后顺序，但是顺序不可控，由CPU随机调取，也导致了多线程的随机性。

- 多线程的优势：

    - 进程之间不能共享数据存储空间，线程可以共享。
    - 系统创建进程需要重新分配资源，创建线程代价小很多，因此多任务并发时，多线程效率高。
    - Java语言本身内置多线程功能的支持，不是单纯作为底层系统的调度方式，从而简化了系统编程。
    - Notice：多线程是为了同步完成多个任务，不是为了提高程序的运行效率，而是通过提高资源使用效率来提高系统的效率。
******

### 线程的生命周期

![image-20200924173042680](C:\Users\15715\AppData\Roaming\Typora\typora-user-images\image-20200924173042680.png) 


******

### 线程优先级

1. 设置线程的优先级？

```java
Public final void setPriority(int newPriority)
```

2. 取得线程优先级？

```java
Public final int getPriority()
```
3. 优先级别：
    - 最高优先级(10)：public static final int MAX_PRIORITY
    - 中等优先级(5)：public static final int NORM_PRIORITY
    - 最低优先级(1)：public static final int MIN_PRIORITY
    - 默认情况下，每一个线程都会分配一个优先级 NORM_PRIORITY（5）。
    - 具有较高优先级的线程对程序更重要，并且应该在低优先级的线程之前分配处理器资源。但是，线程优先级不能保证线程执行的顺序，而且非常依赖于平台。

4. 范例：(测试优先级)
```java
Public class MyThread implements Runable{//runnable子接口
    @override
	Public void run（）{
    	for(int i = 0;i<1000;i++){
        	try{
            	Thread.sleep(500);
        	}catch(Exception e){
            	e.printStatckTrace();
        	}
        	System.out.println(Thread.currentThread().getName()+”,x=”+i);
    	}
	}
}

Public class TestDemo{
    Public void main(String[] args)throws Exception{

	MyThread mt = new MyThread();

	Thread t1 = new Thread(mt,”Thread A”);

	Thread t2 = new Thread(mt,”Thread B”);

	Thread t3 = new Thread(mt,”Thread C”);

	T1.setPriority(Thread.MAX_PRIORITY);

	T2.setPriority(Thread.MIN_PRIORITY);

	T3.setPriority(Thread.MIN_PRIORITY);

	T1.start();

	T2.start();

	T3.start();

}

}


Console:

	Thread C,x=0

	Thread A,x=0

	Thread B,x=0

	Thread C,x=1

	Thread B,x=1

	Thread A,x=1
```
******

### 创建线程的多种方式

- 创建线程有几种方式？
    - 实现Runable 接口创建线程：
        - 定义Class A implements Runable{@override public void run(){}}
        - 创建线程Thread B = new Thread（Runable A,String ThreadName）;
        - 线程启动 B.start();
    - 继承Thread 创建线程：
        - 继承thread：Class C extends Thread{}
        - 重写thread方法：run();start();

    - Callable和Future创建线程：
    >
	    ```java
        public class CallableThreadTest implements Callable<Integer> { 
			public static void main(String[] args) {
		        CallableThreadTest ctt = new CallableThreadTest();
				FutureTask<Integer> ft = new FutureTask<>(ctt);
				for(int i = 0;i < 100;i++) {
					System.out.println(Thread.currentThread().getName()+" 的循环变量i的值"+i);
 					if(i==20) { 
						new Thread(ft,"有返回值的线程").start(); 
					} 
				} 
				try { 
					System.out.println("子线程的返回值："+ft.get());
				} catch (InterruptedException e) { 
				e.printStackTrace(); 
				} catch (ExecutionException e) {
				e.printStackTrace(); } 
			} 
			@Override 
			public Integer call() throws Exception { 
				int i = 0;
 		for(;i<100;i++) { 
					System.out.println(Thread.currentThread().getName()+""+i);} 
				return i; 
		    } 
		}
		```

******

### 线程的主要概念

- 线程同步
    - What？什么是线程同步
        - 线程同步字面意思与实际操作方式相反，其真实含义为“排队”，几个线程之间要排队，一个一个对共享资源进行操作，不能同时操作。

    - Why？为什么使用线程同步
        - 当多个线程同时读写一份共享资源的时候，可能会引起冲突，会造成“丢失数据”、“数据失真”等问题，这个时候需要引入线程“同步”机制，即各个线程之间进行排队。

    - How？怎么样使用线程同步

        - wait():使一个线程处于等待状态，并且释放所持有的对象的lock。
        - sleep():使一个正在运行的线程处于睡眠状态，是一个静态方法，调用此方法要捕捉InterruptedException异常。
        
        - notify():唤醒一个处于等待状态的线程，注意的是在调用此方法的时候，并不能确切的唤醒某一个等待状态的线程，而是由JVM确定唤醒哪个线程，而且不是按优先级。
        - notityAll ():唤醒所有处入等待状态的线程，注意并不是给所有唤醒线程一个对象的锁，而是让它们竞争。

- 线程间通信

    - What？什么是线程间通信

        - JVM中线程的数据区和堆区域是共享的，多个线程处理同一个共享资源时，需要进行通讯和数据交换避免对同一个变量的使用和操作。

    - Why？为什么需要使用线程间通信

        - 多个线程并发执行时，默认情况下CPU是随机切换线程的，当我们需要使用多线程共同完成一个任务，并希望有序的进行，那么多个线程之间需要一些协调通信，以此来达到多个线程共同操作同一份数据。

        - 优点：多线程之间的通信能够避免对同一共享变量的争夺。

    - How？线程间通信如何进行

        - Wait():当前线程等待。线程调用wait方法释放其对锁的拥有权。同时会在等待的位置加一个标志，之后notify唤醒线程是，能从当前位置获得锁的拥有权，变成就绪状态。Wait()调用必须放在synchronized方法或者synchronized块中。在哪里等待被唤醒时，就在哪里执行。
        - notify()/notifyAll():唤醒当前等待对象的锁的线程/唤醒在此对象监视器上的等待的所有线程。当执行notify/notifyAll方法时，会唤醒一个处于等待该 对象锁 的线程，然后继续往下执行，直到执行完退出对象锁锁住的区域（synchronized修饰的代码块）后再释放锁

    - 总结：生产者消费者之间就是运用了wait()和notify()这两个方法，通过通信的沉睡与唤醒机制来完成两个不同线程操作统一数据之间的通信。

- 线程死锁

    - What？什么是线程死锁

        - 所谓死锁是指多个线程因竞争资源而造成的一种僵局（互相等待），若无外力作用，这些进程都将无法向前推进。

    - Why？为什么会出现线程死锁

        - 系统资源的竞争：
        - 进程推进顺序非法：进程在运行过程中，请求和释放资源的顺序不当，也同样会导致死锁
        -  死锁产生的必要条件（必须满足一下四个条件，只要其中任一条件不成立，死锁就不会发生）
            -  互斥条件: 在一段时间内某 资源仅为一个进程所占有。此时若有其他进程请求该资源，则请求进程只能等待
            -  不剥夺条件: 进程所获得的资源在未使用完毕之前，不能被其他进程强行夺走，即只能 由获得该资源的进程自己来释放（只能是主动释放)。
            -  请求和保持条件: 进程已经保持了至少一个资源，但又提出了新的资源请求，而该资源 已被其他进程占有，此时请求进程被阻塞，但对自己已获得的资源保持不放。
            -  循环等待条件: 存在一种进程资源的循环等待链，链中每一个进程已获得的资源同时被 链中下一个进程所请求。

    - How？如何避免线程死锁
        - 加锁顺序：线程按照一定的顺序加锁
        - 加锁时限：线程尝试获取锁的时候加上一定的实现，超过实现则放弃对该锁的请求，并释放自己占有的锁。
        - 死锁检测：

- 线程控制：挂起、停止和恢复
    - Join()
    - Sleep()(休眠)
    - Yield()（让步）
    - Suspend()（挂起）：容易造成死锁，不建议使用
    - Resume()（恢复）：容易造成死锁不建议使用
******

## TCP/UDP

### TCP/UDP/HTTP

- what？什么是TCP

    - TCP/IP:是供已连接Internet的计算机进行通信的协议。

    - 指传输控制协议/国际协议（Transmission Control Protocol/Internet Protocol）

- TCP（内部包含）

    - TCP(传输控制协议)-应用程序之间通信

    - UDP(用户数据报协议)-应用程序之间的简单通信

    - IP(网际协议)- 计算机之间的通信

    - ICMP(英特网消息控制协议)-针对错误和状态

    - DHCP(动态主机配置协议)-针对动态寻址

- 协议

    - HTTP-超文本传输协议（Hyper Text Transfer Protocol）：HTTP 负责 web 服务器与 web 浏览器之间的通信。HTTP 用于从 web 客户端（浏览器）向 web 服务器发送请求，并从 web 服务器向 web 客户端返回内容（网页）。

    - HTTPS- 安全的 HTTP（HTTP Secure）：HTTPS 负责在 web 服务器和 web 浏览器之间的安全通信。作为有代表性的应用，HTTPS 会用于处理信用卡交易和其他的敏感数据。

    - SSL- 安全套接字层（Secure Sockets Layer）：SSL 协议用于为安全数据传输加密数据。

    - SMTP- 简易邮件传输协议（Simple Mail Transfer Protocol）：SMTP 用于电子邮件的传输。

    - MIME - 多用途因特网邮件扩展（Multi-purpose Internet Mail Extensions）：MIME 协议使 SMTP 有能力通过 TCP/IP 网络传输多媒体文件，包括声音、视频和二进制数据。

    - IMAP - 因特网消息访问协议（Internet Message Access Protocol）：IMAP 用于存储和取回电子邮件。

    - POP - 邮局协议（Post Office Protocol）：POP 用于从电子邮件服务器向个人电脑下载电子邮件。

    - FTP - 文件传输协议（File Transfer Protocol）：FTP 负责计算机之间的文件传输。

    - NTP - 网络时间协议（Network Time Protocol）：NTP 用于在计算机之间同步时间（钟）。

    - DHCP - 动态主机配置协议（Dynamic Host Configuration Protocol）：DHCP 用于向网络中的计算机分配动态 IP 地址。

    - SNMP - 简单网络管理协议（Simple Network Management Protocol）：SNMP 用于计算机网络的管理。

    - LDAP - 轻量级的目录访问协议（Lightweight Directory Access Protocol）：LDAP 用于从因特网搜集关于用户和电子邮件地址的信息。

    - ICMP - 因特网消息控制协议（Internet Control Message Protocol）：ICMP 负责网络中的错误处理。

    - ARP - 地址解析协议（Address Resolution Protocol）：ARP - 用于通过 IP 来查找基于 IP 地址的计算机网卡的硬件地址。

    - RARP - 反向地址转换协议（Reverse Address Resolution Protocol）：RARP 用于通过 IP 查找基于硬件地址的计算机网卡的 IP 地址。

    - BOOTP - 自举协议（Boot Protocol）：BOOTP 用于从网络启动计算机。

    - PPTP - 点对点隧道协议（Point to Point Tunneling Protocol）

    - PPTP 用于私人网络之间的连接（隧道）。

- Http

    - What is http？：HTTP是一个基于TCP/IP通信协议来传递数据（HTML 文件, 图片文件, 查询结果等）的协议。

    - How？use http：

        - HTTP协议作用于客户端-服务端架构上
        - 浏览器作为HTTP客户端通过URL向HTTP服务端即WEB服务器发送所有请求。
        -  WEB服务器：
            -  Apache服务器
            -  IIS服务器（Internet Information Service）等
        -  HTTP 3点注意事项：
            -  HTTP是无连接
            -  HTTP是媒体独立的
            -  HTTP是无状态
            -  HTTP协议通信流程：
            -  ![image-20200924172936118](C:\Users\15715\AppData\Roaming\Typora\typora-user-images\image-20200924172936118.png)
******

- HTTP消息结构：
    - 客户端请求消息格式：（请求行、请求头、空行、请求体）：
        -  GET /hello.txt HTTP/1.1         请求头
        -  User-Agent:curl/7.16.3 libcurl/7.16.3 OpenSSL/0.9.7l zlib/1.2.3
        -  Host: www.example.com
        -  Accept-Language: en, mi


    -  服务器响应消息格式：（状态行、消息报头、空行和响应正文）
        -  HTTP/1.1 200 OK       --------------------状态行
        -  Date: Mon, 27 Jul 2009 12:28:53 GMT      --|
        -  Server: Apache								  --|
        -  Last-Modified: Wed, 22 Jul 2009 19:15:56 GMT --|
        -  ETag: "34aa387-d-1568eb00"			    --|à消息报头
        -  Accept-Ranges: bytes							  --|
        -  Content-Length: 51              --|
        -  Vary: Accept-Encoding						  --|
        -  Content-Type: text/plain						  --|

- HTTP请求方法

| 序号 | 方法    | 描述                                                         |
| ---- | ------- | ------------------------------------------------------------ |
| 1    | GET     | 请求指定的页面信息，并返回实体主体。                         |
| 2    | HEAD    | 类似于 GET 请求，只不过返回的响应中没有具体的内容，用于获取报头 |
| 3    | POST    | 向指定资源提交数据进行处理请求（例如提交表单或者上传文件）。数据被包含在请求体中。POST 请求可能会导致新的资源的建立和/或已有资源的修改。 |
| 4    | PUT     | 从客户端向服务器传送的数据取代指定的文档的内容。             |
| 5    | DELETE  | 请求服务器删除指定的页面。                                   |
| 6    | CONNECT | HTTP/1.1 协议中预留给能够将连接改为管道方式的代理服务器。    |
| 7    | OPTIONS | 允许客户端查看服务器的性能。                                 |
| 8    | TRACE   | 回显服务器收到的请求，主要用于测试或诊断。                   |
| 9    | PATCH   | 是对 PUT 方法的补充，用来对已知资源进行局部更新 。           |


- HTTP响应头信息

| 应答头           | 说明                                                         |
| ---------------- | ------------------------------------------------------------ |
| Allow            | 服务器支持哪些请求方法（如GET、POST等）。                    |
| Content-Encoding | 文档的编码（Encode）方法。只有在解码之后才可以得到Content-Type头指定的内容类型。利用gzip压缩文档能够显著地减少HTML文档的下载时间。Java的GZIPOutputStream可以很方便地进行gzip压缩，但只有Unix上的Netscape和Windows上的IE 4、IE 5才支持它。因此，Servlet应该通过查看Accept-Encoding头（即request.getHeader("Accept-Encoding")）检查浏览器是否支持gzip，为支持gzip的浏览器返回经gzip压缩的HTML页面，为其他浏览器返回普通页面。 |
| Content-Length   | 表示内容长度。只有当浏览器使用持久HTTP连接时才需要这个数据。如果你想要利用持久连接的优势，可以把输出文档写入 ByteArrayOutputStream，完成后查看其大小，然后把该值放入Content-Length头，最后通过byteArrayStream.writeTo(response.getOutputStream()发送内容。 |
| Content-Type     | 表示后面的文档属于什么MIME类型。Servlet默认为text/plain，但通常需要显式地指定为text/html。由于经常要设置Content-Type，因此HttpServletResponse提供了一个专用的方法setContentType。 |
| Date             | 当前的GMT时间。你可以用setDateHeader来设置这个头以避免转换时间格式的麻烦。 |
| Expires          | 应该在什么时候认为文档已经过期，从而不再缓存它？             |
| Last-Modified    | 文档的最后改动时间。客户可以通过If-Modified-Since请求头提供一个日期，该请求将被视为一个条件GET，只有改动时间迟于指定时间的文档才会返回，否则返回一个304（Not Modified）状态。Last-Modified也可用setDateHeader方法来设置。 |
| Location         | 表示客户应当到哪里去提取文档。Location通常不是直接设置的，而是通过HttpServletResponse的sendRedirect方法，该方法同时设置状态代码为302。 |
| Refresh          | 表示浏览器应该在多少时间之后刷新文档，以秒计。除了刷新当前文档之外，你还可以通过setHeader("Refresh", "5; URL=http://host/path")让浏览器读取指定的页面。 注意这种功能通常是通过设置HTML页面HEAD区的＜META HTTP-EQUIV="Refresh" CONTENT="5;URL=http://host/path"＞实现，这是因为，自动刷新或重定向对于那些不能使用CGI或Servlet的HTML编写者十分重要。但是，对于Servlet来说，直接设置Refresh头更加方便。  注意Refresh的意义是"N秒之后刷新本页面或访问指定页面"，而不是"每隔N秒刷新本页面或访问指定页面"。因此，连续刷新要求每次都发送一个Refresh头，而发送204状态代码则可以阻止浏览器继续刷新，不管是使用Refresh头还是＜META HTTP-EQUIV="Refresh" ...＞。  注意Refresh头不属于HTTP 1.1正式规范的一部分，而是一个扩展，但Netscape和IE都支持它。 |
| Server           | 服务器名字。Servlet一般不设置这个值，而是由Web服务器自己设置。 |
| Set-Cookie       | 设置和页面关联的Cookie。Servlet不应使用response.setHeader("Set-Cookie", ...)，而是应使用HttpServletResponse提供的专用方法addCookie。参见下文有关Cookie设置的讨论。 |
| WWW-Authenticate | 客户应该在Authorization头中提供什么类型的授权信息？在包含401（Unauthorized）状态行的应答中这个头是必需的。例如，response.setHeader("WWW-Authenticate", "BASIC realm=＼"executives＼"")。 注意Servlet一般不进行这方面的处理，而是让Web服务器的专门机制来控制受密码保护页面的访问（例如.htaccess）。 |


-  HTTP状态码：
    -  200 - 请求成功
    -  301 - 资源（网页等）被永久转移到其它URL
    -  404 - 请求的资源（网页等）不存在
    -  500 - 内部服务器错误

| 分类 | 分类描述                                       |
| ---- | ---------------------------------------------- |
| 1    | 信息，服务器收到请求，需要请求者继续执行操作   |
| 2    | 成功，操作被成功接收并处理                     |
| 3    | 重定向，需要进一步的操作以完成请求             |
| 4    | 客户端错误，请求包含语法错误或无法完成请求     |
| 5    | 服务器错误，服务器在处理请求的过程中发生了错误 |


******


| 状态码 | 状态码英文名称                  | 中文描述                                                     |
| ------ | ------------------------------- | ------------------------------------------------------------ |
| 100    | Continue                        | 继续。[客户端](http://www.dreamdu.com/webbuild/client_vs_server/)应继续其请求 |
| 101    | Switching Protocols             | 切换协议。服务器根据客户端的请求切换协议。只能切换到更高级的协议，例如，切换到HTTP的新版本协议 |
|        |                                 |                                                              |
| 200    | OK                              | 请求成功。一般用于GET与POST请求                              |
| 201    | Created                         | 已创建。成功请求并创建了新的资源                             |
| 202    | Accepted                        | 已接受。已经接受请求，但未处理完成                           |
| 203    | Non-Authoritative Information   | 非授权信息。请求成功。但返回的meta信息不在原始的服务器，而是一个副本 |
| 204    | No Content                      | 无内容。服务器成功处理，但未返回内容。在未更新网页的情况下，可确保浏览器继续显示当前文档 |
| 205    | Reset Content                   | 重置内容。服务器处理成功，用户终端（例如：浏览器）应重置文档视图。可通过此返回码清除浏览器的表单域 |
| 206    | Partial Content                 | 部分内容。服务器成功处理了部分GET请求                        |
|        |                                 |                                                              |
| 300    | Multiple Choices                | 多种选择。请求的资源可包括多个位置，相应可返回一个资源特征与地址的列表用于用户终端（例如：浏览器）选择 |
| 301    | Moved Permanently               | 永久移动。请求的资源已被永久的移动到新URI，返回信息会包括新的URI，浏览器会自动定向到新URI。今后任何新的请求都应使用新的URI代替 |
| 302    | Found                           | 临时移动。与301类似。但资源只是临时被移动。客户端应继续使用原有URI |
| 303    | See Other                       | 查看其它地址。与301类似。使用GET和POST请求查看               |
| 304    | Not Modified                    | 未修改。所请求的资源未修改，服务器返回此状态码时，不会返回任何资源。客户端通常会缓存访问过的资源，通过提供一个头信息指出客户端希望只返回在指定日期之后修改的资源 |
| 305    | Use Proxy                       | 使用代理。所请求的资源必须通过代理访问                       |
| 306    | Unused                          | 已经被废弃的HTTP状态码                                       |
| 307    | Temporary Redirect              | 临时重定向。与302类似。使用GET请求重定向                     |
|        |                                 |                                                              |
| 400    | Bad Request                     | 客户端请求的语法错误，服务器无法理解                         |
| 401    | Unauthorized                    | 请求要求用户的身份认证                                       |
| 402    | Payment Required                | 保留，将来使用                                               |
| 403    | Forbidden                       | 服务器理解请求客户端的请求，但是拒绝执行此请求               |
| 404    | Not Found                       | 服务器无法根据客户端的请求找到资源（网页）。通过此代码，网站设计人员可设置"您所请求的资源无法找到"的个性页面 |
| 405    | Method Not Allowed              | 客户端请求中的方法被禁止                                     |
| 406    | Not Acceptable                  | 服务器无法根据客户端请求的内容特性完成请求                   |
| 407    | Proxy Authentication Required   | 请求要求代理的身份认证，与401类似，但请求者应当使用代理进行授权 |
| 408    | Request Time-out                | 服务器等待客户端发送的请求时间过长，超时                     |
| 409    | Conflict                        | 服务器完成客户端的 PUT 请求时可能返回此代码，服务器处理请求时发生了冲突 |
| 410    | Gone                            | 客户端请求的资源已经不存在。410不同于404，如果资源以前有现在被永久删除了可使用410代码，网站设计人员可通过301代码指定资源的新位置 |
| 411    | Length Required                 | 服务器无法处理客户端发送的不带Content-Length的请求信息       |
| 412    | Precondition Failed             | 客户端请求信息的先决条件错误                                 |
| 413    | Request Entity Too Large        | 由于请求的实体过大，服务器无法处理，因此拒绝请求。为防止客户端的连续请求，服务器可能会关闭连接。如果只是服务器暂时无法处理，则会包含一个Retry-After的响应信息 |
| 414    | Request-URI Too Large           | 请求的URI过长（URI通常为网址），服务器无法处理               |
| 415    | Unsupported Media Type          | 服务器无法处理请求附带的媒体格式                             |
| 416    | Requested range not satisfiable | 客户端请求的范围无效                                         |
| 417    | Expectation Failed              | 服务器无法满足Expect的请求头信息                             |
|        |                                 |                                                              |
| 500    | Internal Server Error           | 服务器内部错误，无法完成请求                                 |
| 501    | Not Implemented                 | 服务器不支持请求的功能，无法完成请求                         |
| 502    | Bad Gateway                     | 作为网关或者代理工作的服务器尝试执行请求时，从远程服务器接收到了一个无效的响应 |
| 503    | Service Unavailable             | 由于超载或系统维护，服务器暂时的无法处理客户端的请求。延时的长度可包含在服务器的Retry-After头信息中 |
| 504    | Gateway Time-out                | 充当网关或代理的服务器，未及时从远端服务器获取请求           |
| 505    | HTTP Version not supported      | 服务器不支持请求的HTTP协议的版本，无法完成处理               |

******

## 邮件发送

## 文档注释

## 数据库连接

- 数据库连接流程：
    - 注册驱动
    - 加载驱动
    - 设置数据库地址
        - 建立数据库连接池
        - 编写sql语句
        - 执行sql语句
        - 断开数据库连接池连接
******
# 分布式

## 分布式事务

- What？什么是分布式事务？：简单的来说分布式事务即为分库分表。单个数据库性能到达瓶颈，对数据库进行物理分区的过程为分布式事务。分布式事务就是指事务的参与者、支持事务的服务器、资源服务器以及事务管理器分别位于不同的分布式系统的不同节点之上。分布式事务就是为了保证不同数据库的数据一致性。

- 分布式理论：当单个数据库性能产生瓶颈的时候，可能会对数据库进行分区（物理分区），分区之后不同的数据库不同的服务器上	，此时单个数据库的ACID不适应这种清苦啊，在此集群环境下很难达到集群的ACID，甚至效率性能大幅度下降，重要的是再很难扩展新的分区了。此时就需要引用一个新的理论来使用这种集群情况：CAP定理。

- CAP定理：由加州肚饿伯克利分校Eric Brewer教授提出，指出WEB服务无法同时满足3个属性：
    - 一致性：客户端知道一系列的操作都会同时发生（生效）

    - 可用性：每个操作都必须以可预期的响应结束

    - 分区容错性：及时出现单组件无法可用，操作依然可以完成。

具体的将在分布式系统中，在任何数据库设计中，一个WEB应用至多只能同时支持上面两个属性。设计人员必须在一致性和可用性之间做出选择。

- BASE理论：分布式系统中追求的是可用性，比一致性更加重要，BASE理论来实现高可用性。核心思想是：我们无法做到羟乙酯，单每个应用都可以根据自身的业务特点，采用适当的方式使系统达到最终一致性。

    - Why？为什么要用分布式事务？（分布式产生的原因）：
        - 数据库分库分表：当数据库单表一年产生的数据超过1000W，那么就要考虑分库分表。
        - 应用SOA化：所谓的SOA化，就是业务的服务化。比如原来单机支撑了整个电商网站，现在对整个网站进行拆解，分离出了订单中心、用户中心、库存中心。对于订单中心，有专门的数据库存储订单信息，用户中心也有专门的数据库存储用户信息，库存中心也会有专门的数据库存储库存信息。这时候如果要同时对订单和库存进行操作，那么就会涉及到订单数据库和库存数据库，为了保证数据一致性，就需要用到分布式事务。

    - How？怎么实现分布式事务（分布式事务的解决方案）
        - 两阶段提交2PC：2PC效率很低，对高并发很不友好
        - 补偿事务TCC：所谓的TCC编程模式，也是两阶段提交的一个变种。TCC提供了一个编程框架，将整个业务逻辑分为三块：Try、Confirm和Cancel三个操作。以在线下单为例，Try阶段会去扣库存，Confirm阶段则是去更新订单状态，如果更新订单失败，则进入Cancel阶段，会去恢复库存。总之，TCC就是通过代码人为实现了两阶段提交，不同的业务场景所写的代码都不一样，复杂度也不一样，因此，这种模式并不能很好地被复用。
        - 本地消息表（异步确保）
        - MQ事务消息
        - Sagas事务模型

******

## 事务特性（ACID）

- 原子性（A）：所谓的原子性就是说，在整个事务中的所有操作，要么全部完成，要么全部不做，没有中间状态。事务在执行中发生错误，所有的操作都会被回滚，整个事务就像从没被执行过一样。

- 一致性（C）：事务的执行必须保证系统的一致性

- 隔离性（I）：隔离性就是说，事务与事务之间不会互相影响，一个事务的中间状态不会被其他事务感知

- 持久性（D）：持久性，就是说一旦事务完成了，那么事务对数据所做的变更就完全保存在了数据库中，即使发生停电，系统宕机也是如此。
******

# 数据库

## 数据库sql语句优化

-  避免在列上做运算，可能会导致索引失败

- 使用join时应该小结果集驱动大结果集，同时把复杂的join查询拆分成多个query，不然join越多表，会导致越多的锁定和堵塞。

- 注意like模糊查询的使用，避免使用%%

- 不要使用select  节省内存

- 使用批量插入语句，节省交互

- Limit基数比较大时，使用between  and

- 不要使用rand函数随机获取记录

- 避免使用null，建表时，尽量设置not nul，提高查询性能

- 不要使用count（id），应该使用count（）

- 不要做无谓的排序，尽可能在索引中完成排序

- From语句中一定不要使用子查询

- 使用更多的where加以限制，缩小查找范围

- 合理运用索引

- 使用explain查看sql性能

- 选择正确的存储引擎

- 固定表的长度

- 使用一个对象关系映射器

- 拆分大的DELETE或INSERT语句

- 垂直分库：“垂直分割”是一种把数据库中的表按列变成几张表的方法，这样可以降低表的复杂度和字段的数目，从而达到优化的目的。

- 水平分库：“水平分割”是一种把数据库中的表按行变成几张表的方法，这样可以降低表的复杂度和字段的数目，从而达到优化的目的。
******

## 关系型数据库

### Oracle

### Mysql

- mysql存储引擎引擎：

![image-20200924172804682](C:\Users\15715\AppData\Roaming\Typora\typora-user-images\image-20200924172804682.png)

 

### Postgresql

## 非关系型数据库

### Redis

### MongoDB

关注 MongoDB 基础以及 Spring 全家桶的整合方案 Spring Data MongoDB 的使用。

1. 谈谈对MongoDB的理解？

2. MongoDB 有哪些特点？

3. MongoDB 都有哪些主要功能？

4. 说说你知道的 MongoDB 适用场景。

5. 关闭 MongoDB 服务的命令是？

6. MongoDB 创建数据库的命令是什么？

******

### HBase

## 数据库搜索引擎

## 分库分表

### 什么是分库分表

- 分库

    - 垂直分库：是指按照业务将表进行分类，分布到不同的数据库上面，每个库可以放不同的服务器上，它的核心理念是专库专用。

    - 水平分库：把同一个表的数据按一定规则拆分到不同的数据库中，每个库可以放不同的服务器上

- 分表

    - 垂直分表：将一个表按照字段分成多表，每个表存储其中一部分字段

    - 水平分表：在同一个数据库内，把同一个表的数据按一定规则拆到多个表中

******

### MySql分库分表

- MySql垂直分库：“垂直分割”是一种把数据库中的表按列变成几张表的方法，这样可以降低表的复杂度和字段的数目，从而达到优化的目的。

- MySql水平分库：“水平分割”是一种把数据库中的表按行变成几张表的方法，这样可以降低表的复杂度和字段的数目，从而达到优化的目的。

- Mycat分库：

    - 什么是MyCat：

MyCat 是目前最流行的基于 java 语言编写的数据库中间件，是一个实现了 MySQL 协议的服务器，前端用户可以把它看作是一个数据库代理，用 MySQL 客户端工具和命令行访问，而其后端可以用 MySQL 原生协议与多个 MySQL 服务器通信，也可以用 JDBC 协议与大多数主流数据库服务器通信，其核心功能是分库分表。配合数据库的主从模式还可实现读写分离。

MyCat 是基于阿里开源的 Cobar 产品而研发，Cobar 的稳定性、可靠性、优秀的架构和性能以及众多成熟的使用案例使得 MyCat 变得非常的强大.MyCat 发展到目前的版本，已经不是一个单纯的 MySQL 代理了，它的后端可以支持MySQL、SQL Server、Oracle、DB2、PostgreSQL 等主流数据库，也支持 MongoDB 这种新型NoSQL 方式的存储，未来还会支持更多类型的存储。而在最终用户看来，无论是那种存储方式，在 MyCat 里，都是一个传统的数据库表，支持标准的 SQL 语句进行数据的操作，这样一来，对前端业务系统来说，可以大幅降低开发难度，提升开发速度。

- MyCat有哪些作用

![image-20200924172838953](C:\Users\15715\AppData\Roaming\Typora\typora-user-images\image-20200924172838953.png)

- Mycat（原理）

    - MyCat技术原理中最重要的一个动词是“拦截”，它拦截了用户发送过来的SQL语句，首先对SQL语句做了一些特定的分析：如分片分析、路由分析、读写分离分析、缓存分析等，然后将此SQL发往后端的真实数据库，并将返回的结果做适当的处理，最终再返回给用户。

![image-20200924172850915](C:\Users\15715\AppData\Roaming\Typora\typora-user-images\image-20200924172850915.png)

- How 如何使用MyCat分库分表




******

# 缓存

## Redis

1. 谈谈你对 Redis 的理解。

2. 简单说说 Redis 的实现原理。
******

# 消息

## MQ

# 检索

## 搜索引擎

# JavaEE

## Servlet

## Socket

# 网关

## Nginx

1. Nginx 反向代理实现高并发的具体步骤是什么？

2. Nginx 搭建Tomcat 集群的核心配置应该怎么写？

3. 

******

# Mybatis

### Mybatis

Mybatis在实际项目开发中会与springMVC整合使用

1. 什么是mybatis（谈谈对mybatis的理解）？

2. MyBatis 接口绑定的优缺点是什么？

3. 实现MyBatis 接口绑定分别有哪几种方式？

4. MyBatis 如何实现一对一关联关系？

5. MyBatis 如何实现一对多关联关系？

6. 说说MyBatis 动态SQL的具体步骤？

7. MyBatis 和 Hibernate 的区别是什么？

8. MyBatis 如何实现模糊查询？
******

# Spring

### Spring

- 什么是spring？

(1) Spring框架是 Rod Johnson开发，是一个非常强大的控制反转框架，帮助分离项目组件之间的依赖关系。

- 什么是springIOC?

- 什么是springAOP?

- Spring AOP 的原理是什么？都有哪些具体的应用场景？

- Ioc属于那种设计模式？

- SpringIOC && DI有什么区别？

- IOC容器的原理？

- Bean 的scope 有几种类型，详细举例

- 说说IOC中的继承和java中的继承有什么区别？

- IoC 中 car 对象的配置如下，现在要添加 user 对象，并且将 car 注入到 user 中，正确的配置是？

-  <bean id="car" class="com.southwind.entity.Car"></bean>

- 请分别写出 IoC 静态工厂方法和实例工厂方法的配置。

- IoC 自动装载有几种方式？

- 介绍一下 Spring 框架中 bean 的生命周期。

- IoC 容器自动完成装载，默认的方式是？

- 谈谈你对 Spring Data JPA 的理解？

- Spring Data JPA 删除多条记录并返回的代码是？

- 谈谈 Spring Data JPA 的底层实现

******

### SpringMVC

- 什么是MVC?

- 什么是springMVC？简单介绍下对springmvc的理解

-  Springmvc的优缺点？

-  SpringMVC 有哪些核心组件？

-  SpringMVC 的实现流程是什么？

-  SpringMVC 如何设定重定向和转发的？

-  如何解决POST和GET 请求中中文乱码问题？

-  @ModelAttribute 注解应该如何使用？

-  说说你对自定义数据类型转换器的理解？

-  使用Hibernate Validator 注解方式校验Emial数据格式应该怎么写？

******

### SpringBoot

-  谈谈你对 Spring Boot 的理解？

(1) Springboot是伴随spring4.0 诞生的，于2014年4月发布第一个版本，是一个内嵌web容器（tomcat/jetty）的可执行程序（jar）的框架。一句话概括的话就是：springboot是一个可执行程序（jar）框架，内嵌了web容器。

-  Spring Boot 的优势是什么？为什么要使用 Spring Boot？

    - Springmvc需要大量的配置文件xml，配置相当繁琐
    - 整合了第三方的框架，配置变简单了。
    - 解决低效的开发效率和部署效率问题
    - Springboot优势：使配置简单、部署简单、编码简单、监控简单。

- Spring Boot 的配置文件有几种格式？区别是什么？

-  谈谈你知道的 Spring Boot 核心注解。

-  如何自动开启 Spring Boot 各个组件？

-  Spring Boot 中 starter 的原理是什么？

-  Spring Boot 不能使用 XML 配置，这句话对吗?

-  什么是 Thymeleaf？

******

### SpringCloud

Spring Cloud 作为 Spring 中最热门的模块，包括服务网关、Ribbon、Feign、	Hystrix、Spring Cloud Config 等，专注实际开发中常用的技能点，同时	具备使用 Spring Cloud 搭建微服务架构的能力。

-  什么是springCloud？

-  Spring Cloud 和 Spring 之间有什么关联关系？

-  Spring Cloud 实现服务注册和发现的原理是什么？

- Ribbon 和 Feign 有什么区别？

-  为什么要使用 Spring Cloud 熔断器，它的作用是什么？

-  什么是 Hystrix？

-  Eureka 和 ZooKeeper 有哪些区别？

-  为什么要使用负载均衡？

-  Spring Cloud 实现服务注册和发现的具体流程是什么？

-  为什么要使用 Spring Cloud ，它有哪些优势？

# Thinking

### 微服务项目实战相关

### 实际工作中 Spring 微服务项目的问题

-  谈谈你对微服务的理解。

-  微服务分别有哪些优点，哪些缺点？

-  谈谈微服务之间是如何实现通信的。

-  Spring Boot 如何集成 MyBatis？

-  Spring Boot 和 Spring Cloud 有哪些区别？

-  使用 layui 的数据表格组件展示业务数据，后台实体类应该如何定义

-  JPA 和 Spring Data JPA 是一回事吗？

-  如果要给项目添加权限管理系统，一般包含哪些需求？

-  微服务架构的拆分都有哪些原则？

-  Feign 和 Ribbon+RestTemplate 的区别是什么？

 

### 限时秒杀

### 12306高并发

### 抢购业务

### GIS匹配

### 定位服务

### 服务器监控

##  

