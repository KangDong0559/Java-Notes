Java目前阶段常用的几个类
====

# Scanner类的使用

> Scanner类的功能：可以实现键盘输入数据，到程序当中。
> Scanner类的使用格式：
>
> - **导包**
> ```java
> import java.util.Scanner;
> ```
> 如果需要使用的目标类，和当前类位于同一个包下，则可以省略导包语句不写
> 只有java.lang包下的内容不需要导包，其他的包都需要import语句  
> - **创建**
>   	**类名称  对象名 =  new  类名称（）;**
> - **使用**
>   	**对象名.成员方法名（）;**
> ```java
> Public int nextInt();		
> //此方法用于录入一个整数
> Public double nextDouble ();
> //此方法用于录入一个小数
> Public String nextLine();	
> //此方法用于录入一个字符串,遇回车键则结束
> Public String next();	
> //此方法用于录入一个字符串,遇 [space键] 或者 [TAB键]则结束.
> ```
***

# Random类的使用

> Random类的功能：用来生成随机数字
> **Random类的使用格式**
> - **导包**
> ```java
> import java.util.Random;
> ```
> - **创建**
> ```java
> Random r = new Random();
> ```
> - **使用**
> ```java
> int num = r.nextInt(); 	
> //此方法用于获取一个随机的int数字
> ```
> (此随机数字范围是int所有数字的范围)
>            		int num = r.nextInt();
> 		(参数代表了范围,范围从0开始,左闭右开)
***
# ArrayList类的使用

> ArrayList类的功能:	用来作为一个容器	它是长度可以随意变化的数组
> **ArrayList类的使用格式**
> - **导包**
> ```java
> import java.util.ArrayList;
> ```
> - **创建**
> ```java
> ArrayList<E> list = new ArrayList<>();
> ```
> > **<E>** 泛型  .	指:集合内的所有元素 ，均统一是E类型的数据，且不能是基本数据类型。
> >
> > 如果希望向集合ArrayList中存储基本数据类型，必须使用基本类型对应的包装类。
> > ***基本数据类型对应的包装类***
> > 
> > | 基本数据类型 |        包装类         |
> > | :----------: | :-------------------: |
> >  |     byte     |         Byte          |
> > |    short     |         Short         |
> > |   **int**    | **Integer** 【特殊】  |
> > |     long     |         Long          |
> > |    float     |         Float         |
> > |    double    |        Double         |
> > |   **char**   | **Charactor**【特殊】 |
> > |   boolean    |        Boolean        |
> - **使用**
> ```java
> public boolean add(E e)						
> //该方法用于向集合当中添加元素,参数的类型与泛型一致.返回值代表添加动作是否成功
> public void add (int index , E e)			
> //该方法用于向集合当中[指定索引位置]添加元素
> public E get (int index);					
> //该方法用于按索引从集合中获取元素  [参数就是索引编号]  返回值就是对应位置的元素
> public E remove (int index);				
> //该方法用于按索引从集合中删除元素  [参数就是索引编号]  返回值就是被删除的元素
> public boolean remove (object o);			
> //该方法用于删除指定的元素  返回值表示删除是否成功
> public int size ();							
> //该方法用于获取集合的尺寸长度,返回值就是集合中包含的元素个数
> public E set (int index,E element);			
> //该方法用于修改指定位置的元素,且返回被修改的元素
> ```

***

# Arrays类的使用

> Arrays类的构造方法被私有   [不可创建对象] 
>
> 成员方法被 static 修饰
> ```java
> public static String toString (int[] a)						
> //该方法用于返回指定数组的具体内容,用字符串表示.
> public static void sort (int[] a)						
> //该方法用于将指定数组按照数字顺序进行排序.
> public static int binarySearch (int[] a ,int key)		
> //该方法用于利用二分查找法,返回指定元素的索引.
> ```
> ```
> 
> ```

***

# Object类的使用

>Java中所有类的根类 (可以理解为: 所有类都间接或直接继承了Object类)
>
>即:	所有类都不用导包 , 可以直接使用Object类中的非私有化成员
> ```java
> public  String  toString();				
> //该方法在类中覆写,进而打印对象名的时候可以方便查看对象中的内容.
> public boolean equals (Object obj){		
> //该方法在类中覆写,进而比较的是这两个对象的内容.
> public class getClass();				
> //该方法用于获取一个类的字节码对象
> ```
> ***如果一个类没用重写equals方法,比较的是这两个对象的地址值.***
> ***如果一个类中重写了equals方法,比较的是这两个对象的内容.***
> ***同一个类的两个字节码对象一定相等***

***

# Objects类的使用

> ```java
> public static String toString(传入对象)					
> //该方法用于将参数中对象返回为字符串.
> public static String toString(传入对象,默认字符串)		
> //该方法用于将参数对象返回为字符串.
> //若参数对象为null,则返回为默认字符串.
> public static Boolean isNull(传入对象)			 		
> //该方法用于判断对象是否为null.
> public static Boolean nonNull(传入对象)					
> //该方法用于判断对象是否不为null.
> ```

***

# String类的使用

> String 是一个不可改变的字符序列
> Java中所有的字符串字面值(如:”ABC”)都作为此类的实例实现.
> **(即: 用双引号引起来的内容,都是String类的对象).**
> > 1.字符串是一个常量,被创建后 其值不可改变. 字符串是一个不可改变的字符序列.
> > 2.字符串可以共享.
> - String 类的构造方法
> - - 空参构造
> ```java
> public String();		
> //--->创建一个字符串对象,内容为空
> ```
> - - 有参构造
> ```java
> public String (byte[] byte);							
> //--->把一个字节数组封装成为一个字符串对象
> public String (byte[] byte ,int offset,int length)		
> //--->把字节数组的一部分封装成为一个字符串对象
> public String (char[] value);							
> //--->把一个字符数组封装成为一个字符串对象
> public String (char[] value, int offset, int count);	
> //--->把一个字符数组的一部分封装成为一个字符串对象
> public String (String original);						
> //--->把一个字符串封装成为一个字符串对象.
> ```
> - 创建字符串对象的区别和对比:
> >1. 用双引号创建的对象,只要字符串序列相同,JVM只会在程序中创建唯一一个字符串对象.并且在**字符串常量池**中进行维护.(***当使用双引号创建字符串对象的时候,系统会检查该字符串在字符串常量池中是否已存在***)																*字符串常量池存在于堆内存中*
> >2. 双引号创建的字符串对象可以在程序中进行**复用**
> >3. 通过new创建的字符串对象,每一次new创建都会开辟空间,即使字符串序列都相同,但地址值都不同.--->此方法创建的字符串对象,存储在堆内存当中
> - String类的特点
>
> > 1. Java中所有的双引号字符串,都是String类的对象
> > 2. 字符串是一个不可改变的序列
> > 3. 字符串对象可以共享
> 当字符串对象使用+号拼接的时候,系统底层会自动创建一个`StringBuilder`对象
> 然后调用其`append方法`完成拼接
> 再调用`toString`方法转换为`String`类型
> 并返回给拼接处.
> - [ ] Java中存在**常量优化机制**.  **?**
> - 字符串的比较
> > 要比较字符串内容是否相同,需要通过`equals();`或者`equalsIgnoreCase();`方法来实现.
> >
> > ```java
> > public boolean euqals(Stirng anObject)						
> > //此方法比较内容的时候,比较两个字符串内容是否完全一致.
> > public boolean equalsIgnoreCase(String anotherString);		
> > //此方法比较内容的时候,可以忽略大小写.
> > ```
> - 字符串的遍历
> > 遍历字符串的方法:(字符串的索引同数组)
> >
> > 字符串的长度:---->通过`length();方法`获取.
> > ```java
> > public char charAt (int index);			//返回指定索引值的char值.
> > public char[] toCharArray();			//将字符串转换为一个新的字符数组.
> > ```
> >
> > - - - (只有字符数组直接打印的时候,不是打印地址值,而是打印数组内容.)
> - 截取字符串的方法
>
> > ```java
> > public String substring(int beginIndex);			
> > //此方法从beginIndex索引位置,向后一直截取到末尾,并返回一个字符串.(含头)
> > public String substring(int beginIndex , int endIndex);
> > //此方法从beginIndex索引位置开始截取,向后截取到endIndex索引位置,并返回一个新的字符串.(含头不含尾)
> > ```
> >
>
> - 字符串的转换
>
> > ```java
> > public String toLowerCase();
> > //此方法用于将字符串内的字母全部转换为小写字母.
> > public String toUpperCase();
> > //此方法用于将字符串内的字母全部转换为大写字母.
> > ```
>
> - 字符串的替换
>
> > ```java 
> > public String replace(CharSequence target,CharSequnce replacement);
> > //此方法可将target内容,进行replacement进行替换,并返回新的字符串.
> > public String replaceAll (String regex , String replacement);
> > //此方法把字符串中所有的regex,替换成replacement .
> > public String replaceFirst (String regex, String replacement);
> > //此方法把字符串中第一次出现的regex,替换成replacemen
> > ```
>
> - 切割字符串
>
> > ```java
> > public String[] split (String regex);
> > //此方法可以根据传入的字符串作为规则进行切割,将切割后的内容存入字符串数组中,并返回这个数组.
> > ```

***

# StringBuilder类的使用

> 是一个**可变的字符序列**,可视为一个可以存储任何类型数据的容器,但**均以字符串形式存在**.
>
> 最大程度提高字符串的操作效率
> - StringBuilder的构造方法
> - - 空参构造
>  ```java
> public StringBuilder ();
> //创建一个空白可操作的字符串
>  ```
> - - 有参构造
> ```java
> public StringBuilder(String str);
> //创建一个可变的字符串对象,根据所传入的字符串的内容初始化
> ```
> - 常用方法
> > ```java
> > public StringBuilder append (任意类型);
> > //此方法可以用来添加数据(至字符串末尾),并返回对象本身.
> > public StringBuilder reverse();
> > //此方法返回相反的字符序列.
> > public int length();
> > //此方法用来返回字符的长度.
> > public String toString();
> > //此方法用于将StringBuilder类型转换为String
> > ```
> - String与StringBuilder的转换
> (1) String ===>  StringBulier
> ```java
> //通过调用StringBuilder类的构造方法:
> public StringBuilder(String str);
> //传入String变量做实参
> ```
> ​	(2) StringBuilder ===> String
> ```java
> //利用toString()方法:
> public String toString();
> ```

***

# Math类的使用

> ***一个工具类***	[ 构造方法被私有  不能创建对象 ]
>
> - 成员方法:
> ```java
>  public static int abs (int a)
> //该方法用于返回参数的绝对值.
> public static double ceil(double a)
> //该方法用于将参数向上取整.
>  public static double floor(double a)
> //该方法用于将参数向下取整.
>  public static int round (float a)
> //该方法用于将参数四舍五入.
>  public static int max (int a,int b)
> //该方法用于返回两个int值中的较大值.
>  public static int min (int a,int b)
> //该方法用于返回两个int值中的较小值.
>  public static double pow (double a, double b)
> //该方法用于返回a的b次幂.
>  public static double random ()
> //该方法用于返回double的随机数.  [0.0,1.0)
> ```

***

# System类的使用

> [ 构造方法被私有  不能创建对象 ]
> - 成员方法:
> ```java
>  public static void exit (int status)
> //该方法用于终止当前运行的Java虚拟机.
> //0:表示正常停止.
> public static long currentTimeMills()
> //该方法用于从1970年1月1日起,到当前时间所经过的毫秒时间.
> public static void arraycopy (数据源数组,起始索引,目的地数组,起始索引,拷贝个数)
> //该方法用于拷贝数组.
> ```
***

# BigDecimal类的使用

> ***一个用于进行精确计算的类***	
> - 构造方法 
> ```java
> public BigDecimal (double val ) ;
> //传入double参数
> public BigDeciaml (String val) ;
> //传入String参数
> ***[ 注意 ] : 想要用 BigDecimal 对象 , 则必须使用`String`类型做参数的构造方法 ***
> - 成员方法
> ​```java
> public BigDecimal add (BigDecimal decimal) ;
> //该方法用于两个BigDecimal对象之间进行精确的**加法**运算 
> public BigDecimal subtract (BigDecimal decimal);
> //该方法用于两个BigDecimal对象之间进行精确的**减法**运算
> public BigDecimal multiply (BigDecimal decimal) ;
> //该方法用于两个BigDecimal对象之间进行精确的**乘法**运算
> public BigDecimal divide (BigDecimal decimal) ;
> //该方法用于两个BigDecimal对象之间进行精确的**除法**运算
> //当这两个对象做除法,无法除尽时,使用该方法会出现异常.
> public BigDecimal divide (BigDecimal decimal , int 精确几位 , 舍入模式);
> //舍入模式常用的三个参数:
> 		// ROUNE_UP			---->		 进一法
> 		// ROUND_FLOOR		---->		去尾法
> 		// ROUND_HALF_UP	---->		四舍五入
> ```

***

# 基本数据类型包装类 ----以Integer为例

> 包装类的作用 : 将基本数据类型和字符串之间做转换 
> 将基本数据类型封装成对象的好处在于 :
> 		可以在对象中定义更多的方法和功能 , 对数据做操作.
>
> - 构造方法 
>   ```java
>   public Integer (int value) ;
>   //根据 int 数据创建 Integer 对象 (已过时)
>   public Integer (String value ) ;
>   //根据 String 对象 创建 Integer 对象 (已过时) 
>   public static Integer valueOf ( int i );
>   //返回与参数 i 值 相对应的 Integer 对象
>   public static Integer valueOf ( String s ) ;
>   //返回与参数 s 值相对应的 Integer 对象.
>   > Integer的自动装箱和自动拆箱
>   > Integer i1 = 100; (100 是int数据,这里Java底层自动调用了`valueOf`方法)
>   > int i2 = i1 ; 即是自动拆箱
>   ```
>  - 成员方法
>  ```java
>  public static int parseInt ();
>  //此方法用于将字符串类型的整数类型数据转换为int类型的整数
>  ```

***

# Date类的使用
> Date类  ---> 代表一个特定的时间 , 精确到毫秒值 .
> 		---> 导包应导入 *java.util.Date* 
> - 构造方法 
> ```java
> public Date () ;
> //创建一个Date对象 , 表示**默认时间**
> public Date (long Date) ;
> //创建一个Date对象 , 表示指定的时间 .** 传入的对象即是显示的时间**
> ```
> - 成员方法
> ```java
> public long getTime ();
> //此方法用于获取当前时间的毫秒值
> public void setTime (long time ) ;
> //此方法用于设置一个时间,传递的是毫秒值 
> ```
> - 使用案例 
> ```java
>        Date date = new Date();
>        System.out.println(date);  //打印的是当前电脑设定时间的值.
> 
>       Date date2 = new Date(0L);
>        System.out.println(date2);// Thu Jan 01 08:00:00 CST 1970
>                                  // 1970年01月01日 08:00:00  星期二.
>        /*
>        Thu Jan 01 08:00:00 CST 1970
>        就是计算机的时间原点,经过参数(long date)毫秒值的时间.
>         */
> 
>       //时间原点开始,经过一小时后的时间.
>        Date date3 = new Date(3600L * 1000);
>        System.out.println(date3);
> ```
> ## SimpleDateFormat 类的使用
>
> SimpleDateFormat 类 可以对Date对象进行格式化(format) 和 解析(parse)
> 查API 可知解析格式: 
> 		Y	--->	年
> 		M	--->	月
> 		d	--->	日
> 		H	--->	时	in a day
> 		m	--->	分	in an hour
> 		s	--->	秒	in a minute
>
> - 成员方法
> ```java
> public final String format (Date date ) ;
> //将日期格式化为 日期/时间 的字符串格式
> public Date parse (String source) ;
> //按照给定字符串中解析文本, 输出日期/时间.
> ```
> - 使用案例
> > ```java
> > 	public static void main(String[] args) throws ParseException {
> >        String start = "2020年11月11日 00:00:00";
> >        String end   = "2020年11月11日 00:10:00";
> >
> >        String jia   = "2020年11月11日 00:03:47";
> >        String pi    = "2020年11月11日 00:10:11";
> >        //将时间转化成毫秒值,用于进行时间上的判断;0
> >        //  字符串 --->  解析  --->  date对象  --->  getTime();
> >        SimpleDateFormat sdf = new SimpleDateFormat("yyyy年MM月dd日 HH:mm:ss");
> >        long startTime = sdf.parse(start).getTime();
> >        long endTime = sdf.parse(end).getTime();
> >
> >        long jiaTime = sdf.parse(jia).getTime();
> >        long piTime = sdf.parse(pi).getTime();
> >
> >        //进行判断
> >        if (jiaTime >= startTime && jiaTime <= endTime){
> >            System.out.println("小贾同学参加上了秒杀活动");
> >        }else {
> >            System.out.println("小贾同学没有参加上秒杀活动");
> >        }
> >
> >        if (piTime >= startTime && piTime <= endTime){
> >            System.out.println("小皮同学参加上了秒杀活动");
> >        }else {
> >            System.out.println("小皮同学没有参加上秒杀活动");
> >        }
> >    }	
> >    ```
> ## LocalDate 类的使用
> > LocalDate 表示日期
> ## LocalTime 类的使用
> > LocalTime 表示时间
> ## LocalDateTime 类的使用
> > LocalDateTime 表示日期 + 时间
> > - 构造方法
> > > ```java
> > > public static LocalDateTime now () ;
> > > // 此方法用于获取当前时间
> > > public static LocalDateTime of ( int 年, 月, 日 , 时, 分, 秒)
> > > // 此方法用于使用指定年月日和时分秒初始化一个LocalDateTime对象.
> > > ```
> > - LocalDateTime的成员方法
> > > ```java
> > >  public int getYear ();              
> > >  // 获取年
> > >  public int getMonthValue ();       
> > >   // 获取月份(1-12)
> > >  public int getDayOfMonth ();       
> > >   // 获取月份中的第几天(1-31)
> > >  public int getDayOfYear ();         
> > >  // 获取一年中的第几天(1-366)
> > >  public DayOfWeek get DayOfWeek (); 
> > >   // 获取星期
> > >  public int getMinute ();            
> > >  // 获取分钟
> > >  public int getHour ();             
> > >   // 获取小时
> > >   ```
> > - LocalDateTime的转换方法
> > > ```java
> > > public LocalDate toLocalDate ();
> > > //转换成为一个LocalDate对象
> > > public LocalTime toLocalTime ();
> > > //转换成为一个LocalTime对象
> > > ```
> > - LocalDateTime的增加/减少时间的方法
> > > ```java
> > >  public LocalDateTime plusYear (long years);        
> > >   //添加或者减少[年]
> > >   //这里会返回一个新的LocalDateTime对象.需要定义一个变量进行接收
> > >   .//[注意事项]: 该方法可以接收正数,也可以接收负数.接收负数即是减去x年.
> > >  public LocalDateTime plusMonths (long month);
> > >  public LocalDateTime plusDays (long days);
> > >  public LocalDateTime plusHours (long hours);
> > >  public LocalDateTime plusMinutes (long minutes);
> > >  public LocalDateTime plusSeconds (long seconds);
> > >  public LocalDateTime plusWeeks (long weeks);
> > >  public LocalDateTime minusYears (long years)
> > >  public LocalDateTime minusMonths (long months)
> > >  public LocalDateTime minusDays (long days)
> > >  public LocalDateTime minusHours (long hours)
> > >  public LocalDateTime minusMinutes (long minutes)
> > >  public LocalDateTime minusSeconds (long seconds)
> > >  public LocalDateTime minusWeeks (long weeks)
> > >  ```
> > - 使用案例
> > > ```java
> > > class Demo05LocalDateTimeParseTime {
> > >    /*
> > >     LocalDateTime方法默认打印格式不好看,
> > >     于是可以采取     public String format (指定格式);
> > >                           ---->       将一个LocalDateTime格式化成为一个字符串.
> > >                     public LocalDateTime parse (准备解析的字符串,解析格式);
> > >                            ---->       将一个日期字符串解析成为一个LocalDateTime对象.
> > >                     这两个方法来进行格式化和解析.
> > >     */
> > >    public static void main(String[] args) {
> > >        LocalDateTime localDateTime = LocalDateTime.of(2020, 11, 20, 20, 03);
> > >        System.out.println(localDateTime);
> > >
> > >        //localDateTime.format 的参数是一个DateTimeFormatter对象
> > >        localDateTime.format(DateTimeFormatter.ofPattern("yyyy年MM月dd日 HH:mm:ss"));
> > >
> > >        String s = "2020年11月20日 20:30:00";
> > >        //LocalDateTime.parse 的第一个参数是一个charSequence对象....但可以传入字符串对象
> > >        LocalDateTime.parse(s,DateTimeFormatter.ofPattern("yyyy年MM月dd日 HH:mm:ss"));
> > >    }
> > > }
> > > ```
> > - LocalDateTime的修改方法
> > > ```java
> > >  public LocalDateTime withYear (int year) 
> > >  //直接修改年
> > >  public LocalDateTime withMonth (int month)
> > >  //直接修改月
> > >  public LocalDateTime withDayOfMonth (int dayofmonth)
> > >  直接修改日期(一个月中的第几天)
> > >  public LocalDateTime withDayOfYear (int dayofyear)
> > >   //直接修改日期(一年中的第几天)
> > >  public LocalDateTime withHour (int hour) 
> > >  //直接修改小时
> > >  public LocalDateTime withMinute (int minute)
> > >  //直接修改分钟
> > >  public LocalDateTime withSecond (int second)
> > >  //直接修改秒
> > >  ```
> ## Period 类的使用
>
> > 用于获取<u>以年月日做单位的时间间隔</u>
> - 成员方法
> > ```java
> > public static Period between (开始时间,结束时间) 
> > //计算两个时间的间隔
> > public int getYears()
> > //获得这段时间的年份数
> > public int getMonths() 
> > //获得这段时间的年份数
> > public int getDays()
> > //获得这段时间的年份数
> > public long toTotalMonths()
> > //获得此期间的总月数
> > ***[注意事项]***:Period类中使用的对象时LocalDate
> > ```
> ## Duration 类的使用
>
> > 用于获取<u>以时分秒为单位的时间间隔</u>
> - 成员方法
> > ```java
> > public static Duration between (开始时间,结束时间);
> > //计算两个时间的间隔.
> > public long toSeconds (); 
> > //获取此时间间隔的秒
> > public int toMillis ();
> > //获取此时间间隔的毫秒
> > public int toNanos ();
> > //获取此时间间隔的纳秒
> > ```
> ***[注意事项] ***: Duration 的传入参数是Temporal.
> 			     													 Temporal 是一个接口.
> 			      								已学类中,是 Temporal  实现类 的有:	*LocalDate* 	*LocalTime* 	*LocalDateTime*  

***

# Exception类 (异常)

> 异常指:程序执行过程中出现不正常的情况,最终会导致JVM的非正常停止. (语法错误不再异常体系中.)
> ####  异常的框架体系
>
> ```
> Thorwable 分类: Exception(异常) 指程序本身可以处理的异常问题
> 							--->	RuntimeException及其子类: 运行时期异常
> 							--->	除RuntimeException之外的所有异常: 编译时期异常
> 			  Error (错误)
> ```
>
> ## throws 关键字的使用
>
> throws的作用有:
> > (1) 通知调用者,若进行调用,可能会出现该异常.
> > (2) 如果方法中没有出现异常,则正常运行
> > (3) 如果方法中出现了异常,则将异常交给调用者处理.
> > (4) 如果调用者未作处理,那么将异常交给JAVA虚拟机处理.
> > throws 与 throw 的区别:
> >
> > - throws
> > > (1) 使用位置的不同:用在方法声明后,后跟异常类名
> > > (2) 作用效果的不同:表示声明异常,调用该方法可能会出现该异常
> > - throw
> > > (1) 使用位置的不同:用在方法体内,后跟异常类名
> > > (2) 作用效果的不同:表示手动抛出异常对象,由方法体内的语句进行处理
> > >
> ## Throwable 的成员方法
> > ```java
> > public String getMessage ();
> > //该方法用于以字符串形式返回,此throwable的详细消息
> > public String toString ();
> > //该方法用于以字符串形式返回,此可抛出的异常的简短描述.
> > public void printStackTrace ();
> > //该方法用于将异常的错误信息打印在控制台上.
> > ```
> > - 抛出异常的意义:
> > (1)在方法中,当传递的参数有误,没有继续进行下去的意义了,则采取抛出处理.表示让该方法结束运行.
> > (2)告诉调用者,方法中出现问题.
> ## try...catch的使用
> > 格式: try {
> >            可能出现异常的代码
> >        } catch (异常类名  变量名) {
> >            异常的处理代码
> >        }
> > - 使用案例
> > ```java
> > protected static void Question1() {
> >   	// (1) 如果try中没有遇到问题,该怎么执行?
> >  	// 回答: 程序除了catch内的内容,正常完整执行了.
> >   try {
> >       Scanner sc = new Scanner(System.in);
> >      System.out.println("请输入您的年龄.");
> >      String ag = sc.next();
> >       int age = Integer.parseInt(ag);
> >            System.out.println(age);
> >          System.out.println("测试1");
> >     } catch (NumberFormatException e) {
> >        System.out.println("cath执行了");//没有执行.
> >     }
> >     System.out.println("测试2");
> >    }
> >     protected static void Question2() {
> >         //(2) 如果try中遇到了问题,那么try下面的代码还会执行吗?
> >         //回答:当try语句中出现了异常,那么直接跳转到catch内的代码,然后继续执行外部代码.
> >       try {
> >            Scanner sc = new Scanner(System.in);
> >            System.out.println("请输入您的年龄.");
> >           String ag = sc.next();
> >           int age = Integer.parseInt(ag);
> >            System.out.println(age);
> >            System.out.println("测试1234");//没有执行
> >         } catch (NumberFormatException e) {
> >             System.out.println("cath执行了");//执行了....
> >         }
> >         System.out.println("测试2234");//执行了...
> >     }
> >   protected static void Question3() {
> >   		//(3) 如果出现的问题没有捕获,那么程序如何运行?
> >         // 回答:问题未能成功捕获,则会将出现的异常抛给JVM进行处理.整个方法停止执行.
> >        try {
> >            Scanner sc = new Scanner(System.in);
> >            System.out.println("请输入您的年龄.");
> >            String ag = sc.next();
> >            int age = Integer.parseInt(ag);
> >            System.out.println(age);
> >            System.out.println("测试AA");
> >        } catch (NullPointerException e) {
> >            System.out.println("cath执行了");
> >        }
> >         System.out.println("测试BB");
> >     }
> >    protected static void Question4() {
> >         //(4) 可能同时出现多个异常,应该怎么处理?
> >         //当try正确捕获到第一个异常,整个try语句体不再执行,跳转到catch语句.
> >         //若try正确捕获到第二个异常,则相当于执行catch语句中if判断,匹配异常类后执行其对应的语句.
> >         //如果出现多个异常,那么可以书写多个catch语句;
> >         //如果多个异常之间存在子父类关系,那么父类异常一定要写在下面.
> >         try {
> >             Scanner sc = new Scanner(System.in);
> >             System.out.println("请输入您的年龄.");
> >             String ag = sc.next();
> >             int age = Integer.parseInt(ag);   //异常1:数据格式化异常
> >             System.out.println(age);
> >             System.out.println(2/0);   		 //异常2:数学运算异常
> >             System.out.println("测试QWE");
> >         } catch (NumberFormatException e) {
> >             System.out.println("cath执行了"); //没有执行.
> >         } catch (ArithmeticException e){
> >             System.out.println("数学运算异常被捕获");
> >         }
> >         System.out.println("测试ASD");
> >     }
> > }
> > 
> > ```
> > - try...catch的作用
> > ***让代码继续运行下去.***
> > ###自定义异常
> > 步骤:
> > (1) 定义异常类, 类名见名知意.
    (2) 建立异常关系.
    (3) 空参有参构造.
