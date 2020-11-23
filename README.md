 Java-Notes
 =
personalStudyNotes
-

# Scanner类的使用
<br>Scanner类的功能：可以实现键盘输入数据，到程序当中。
<br>Scanner类的使用格式：
<br>(1)导包
<br>    import java.util.Scanner;
<br>    如果需要使用的目标类，和当前类位于同一个包下，则可以省略导包语句不写。
<br>    只有java.lang包下的内容不需要导包，其他的包都需要import语句。
<br>(2)创建
<br>    类名称  对象名 =  new  类名称（）;
<br>(3)使用
<br>    对象名.成员方法名（）;
<br>Public int nextInt();
<br>(此方法用于录入一个整数
<br>Public double nextDouble ();
<br>此方法用于录入一个小数
<br>Public String nextLine();
<br>此方法用于录入一个字符串,遇回车键则结束.
<br>Public String next();
<br>此方法用于录入一个字符串,遇 空格键 or TAB键则结束.
# Random类的使用
<br>  Random类的功能：用来生成随机数字。
<br>  Random类的使用格式
<br>  (1)导包
<br>      import java.util.Random;
<br>  (2)创建
<br>      Random r = new Random();
<br>  (3)使用
<br>     获取一个随机的int数字:int num = r.nextInt();
<br>    (此随机数字范围是int所有数字的范围)
<br>           int num = r.nextInt();
<br>    (参数代表了范围,范围从0开始,左闭右开)
# ArrayList类的使用
<br>  ArrayList类的功能：作为一个长度可以随意变化的数组。
<br>  ArrayList类的使用格式：
<br>  1.导包
<br>  import java.util.ArrayList;
<br>  2.创建
<br>  ArrayList<E> list = new ArrayList<>();
<br>  <E>(泛型):指集合内的所有元素,均统一是X类型的数据,且不能是基本类型数据.
<br>  如果希望向集合ArrayList当中存储基本数据类型,必须使用基本类型对应的"包装类".
<br>  基本类型            包装类(引用类型,都位于java.long包下)
<br>  byte                Byte
<br>  short               Short
<br>  int                 Integer 【特殊】
<br>  long                Long
<br>  float               Float
<br>  double              Double
<br>  char                Character【特殊】
<br>  boolean             Boolean
<br>  3.使用
<br>  ArrayList当中常用的方法
<br>  (1)add方法:public boolean add (E e);//向集合当中添加元素,参数的类型与泛型一致.返回值代表添加动作是否成功.
<br>       public void add (int index,E  e);//向集合当中指定位置添加元素.
<br>  (2)读取方法:public E get(int index);//从集合中获取元素,参数就是索引编号,返回值就是对应位置的元素.
<br>  (3)删除方法:public E remove(int index);//从集合中删除元素,参数就是索引编号,返回值就是被删除的元素.
<br>       public boolean remove(Object o);//删除指定的元素,返回值表示删除是否成功.
<br>  (4)获取长度:public int size();//获取集合的尺寸长度,返回值就是集合中包含的元素个数.
<br>  (5)修改元素:public E set (int index , E element);//修改指定位置的元素,返回被修改的元素.
# Object类的使用--->类层次的根类(可以理解为所有类的父类)
                    也就不用导包,子类可以直接使用父类中的非私有化成员.
// Public  String  toString();
    该方法在类中覆写,进而打印对象名的时候可以方便查看对象中的内容.
// Public boolean equals (Object obj){
// return (this  ==  obj)
// }
    如果一个类没用重写equals方法,比较的是这两个对象的地址值.
    如果一个类中重写了equals方法,比较的是这两个对象的内容.
    getClass();
    获取一个类的字节码对象.
    同一个类的两个字节码对象一定相等
## String类的使用: --->不可改变的字符序列.
String代表字符串 .
Java中所有的字符串字面值(如:”ABC”)都作为此类的实例实现.
(即: 用双引号引起来的内容,都是String类的对象).
1.字符串是一个常量,被创建后 其值不可改变. 字符串是一个不可改变的字符序列.
2.字符串可以共享.
5.1 String类的构造:
创建String类的对象的方法:1.使用构造方法;2.直接使用双引号;
(1)空参构造:public String();--->创建一个字符串对象,内容为空
(2)有参构造:public String (byte[] byte);
--->把一个字节数组封装成为一个字符串对象
public String (byte[] byte ,int offset,int length)
--->把字节数组的一部分封装成为一个字符串对象
public String (char[] value);
--->把一个字符数组封装成为一个字符串对象
public String (char[] value, int offset, int count);
--->把一个字符数组的一部分封装成为一个字符串对象
public String (String original);
--->把一个字符串封装成为一个字符串对象.
5.2 创建字符串对象的区别和对比:
1.用双引号创建的对象,只要字符串序列相同,JVM只会在程序中创建唯一一个字符串对象.并且在字符串常量池中进行维护.(当使用双引号创建字符串对象的时候,系统会检查该字符串在字符串常量池中是否已存在)字符串常量池存在于方法区(堆内存)中.
双引号创建的字符串对象可以在程序中进行复用.
2.通过new创建的字符串对象,每一次new创建都会开辟空间,即使字符串序列都相同,但地址值都不同.--->此方法创建的字符串对象,存储在堆内存当中.

5.3 String类的特点:
1.Java中所有的双引号字符串,都是String类的对象
2.字符串是一个不可改变的序列
3.字符串对象可以共享.
当字符串对象使用+号拼接的时候,系统底层会自动创建一个StringBuilder对象,然后调用其append方法完成拼接,再调用toString方法转换为String类型,返回给拼接处.
Java中存在常量优化机制.(?)
5.4 字符串的比较:
要比较字符串内容是否相同,需要通过equals();&equalsIgnoreCase();方法来实现.
public boolean euqals(Stirng anObject);
此方法比较内容的时候,比较两个字符串内容是否完全一致.
public boolean equalsIgnoreCase(String anotherString);
此方法比较内容的时候,可以忽略大小写.
5.5 字符串的遍历
遍历字符串的方法:(字符串的索引同数组)
字符串的长度:---->通过length();方法获取.
public char charAt (int index);返回指定索引值的char值.
public char[] toCharArray();将字符串转换为一个新的字符数组.
(只有字符数组直接打印的时候,不是打印地址值,而是打印数组内容.)
5.6 截取字符串的方法
String substring(int beginIndex);
此方法从beginIndex索引位置,向后一直截取到末尾,并返回一个字符串.(含头)
String substring(int beginIndex , int endIndex);
此方法从beginIndex索引位置开始截取,向后截取到endIndex索引位置,并返回一个新的字符串.(含头不含尾)
5.7 字符串的转换
public String toLowerCase();
此方法用于将字符串内的字母全部转换为小写字母.
public String toUpperCase();
此方法用于将字符串内的字母全部转换为大写字母.
5.8 字符串替换
public String replace(CharSequence target,CharSequnce replacement);
此方法可将target内容,进行replacement进行替换,并返回新的字符串.
public String replaceAll (String regex , String replacement);
此方法把字符串中所有的regex,替换成replacement .
public String replaceFirst (String regex, String replacement);
此方法把字符串中第一次出现的regex,替换成replacement	 .
5.9 切割字符串
public String[] split (String regex);
此方法可以根据传入的字符串作为规则进行切割,将切割后的内容存入字符串数组中,并返回这个数组.
6. StringBuilder类的使用 ---->是一个可变的字符序列,可视为一个可以存储任何类型数据的容器,但均					 以字符串形式存在.
最大程度提高字符串的操作效率
6.1 StringBuilder的构造方法
空参构造:--->创建一个空白可操作的字符串.
public StringBuilder ();
有参构造:--->创建一个可变的字符串对象,根据所传入的字符串的内容初始化
public StringBuilder(String str);
6.2 常用方法:
public StringBuilder append (任意类型);
此方法可以用来添加数据(至字符串末尾),并返回对象本身.
public StringBuilder reverse();
此方法返回相反的字符序列.
public int length();
此方法用来返回字符的长度.
public String toString();
此方法用于将StringBuilder类型转换为String.
6.3 String与StringBuilder的转换
(1)String ---> StringBuilder
	通过调用StringBuilder构造方法:
public StringBuilder(String str);--->传入String变量做实参.
(2)StringBuilder ---> String
通过toString()方法即可.
7. Math类的使用 ---> 包含基本数字运算的方法,是一个工具类
Math类不能够创建对象,直接用 Math.方法名 进行调用即可.
7.1 public static int abs (int a)
该方法用于返回参数的绝对值.
7.2 public static double ceil(double a)
该方法用于将参数向上取整.
7.3 public static double floor(double a)
该方法用于将参数向下取整.
7.4 public static int round (float a)
该方法用于将参数四舍五入.
7.5 public static int max (int a,int b)
该方法用于返回两个int值中的较大值.
7.6 public static int min (int a,int b)
该方法用于返回两个int值中的较小值.
7.7 public static double pow (double a, double b)
该方法用于返回a的b次幂.
7.8 public static double random ()
该方法用于返回double的随机数.  [0.0,1.0)
8. Objects类的使用---> 始于JDK1.7
8.1 public static String toString(传入对象)
该方法用于将参数中对象返回为字符串.
8.2 public static String toString(传入对象,默认字符串)
该方法用于将参数对象返回为字符串.
若参数对象为null,则返回为默认字符串.
8.3 public static Boolean isNull(传入对象)
该方法用于判断对象是否为null.
8.4 public static Boolean nonNull(传入对象)
该方法用于判断对象是否不为null.
9. System类的使用---> 
System类也不能创建对象.直接用System.方法名 进行调用即可.
9.1 public static void exit (int status)
该方法用于终止当前运行的Java虚拟机.
0:表示正常停止.
9.2 public static long currentTimeMills()
该方法用于从1970年1月1日起,到当前时间所经过的毫秒时间.
9.3 public static void arraycopy (数据源数组,起始索引,目的地数组,起始索引,拷贝个数)
该方法用于拷贝数组.
10. Arrays类的使用 --->不可创建对象.static修饰
10.1 public static String toString (int[] a)
该方法用于返回指定数组的具体内容,用字符串表示.
10.2 public static void sort (int[] a)
该方法用于将指定数组按照数字顺序进行排序.
10.3 public static int binarySearch (int[] a ,int key)
该方法用于利用二分查找法,返回指定元素的索引.
