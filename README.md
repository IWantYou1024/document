
		【主函数、类名、括号】

第一步学会怎么==调试,检验语法错误
---------------空指针判断
--------乱码不能ctrl+s保存修改------>由小改到大.....备份(复制到txt,改好编码,保存,"修改""保

存)
软件安装:注意最好不要安装在中文目录下,空格,特殊符号

数学 方法==简化程序
【注意定义语句的位置】，int a=3定义全局变量，则全局的，静态的，主函数中
【注意｛｝的位置，特别在循环中】
利用输出语句，输出每一个步骤 ，，【来确定是自己预料的过程结果】
；;注意中英符号：提示找不到符号
注意赋值后，，修改相应字母；
double 类型相加：1.1+2.2=3.3000000003
3, 当父类中没有空参数构造方法的时候，怎么办？
			a: 通过 super(参数) 访问父类有参数的构造方法
			b: 通过 this(参数) 访问本类中其他构造方法
			   注意:[本类中的其他构造方法已经能够正常访问父类构造方法]
		4, super(参数) 与 this(参数) 不能同时在构造方法中存在
代码块：
		局部代码块：定义在方法中的，用来限制变量的作用范围
		构造代码块：定义在类中方法外，用来给对象中的成员初始化赋值
		静态代码块：定义在类中方法外，用来给类的静态成员初始化赋值
		
		
0.5：char c='一';
		System.out.println((int)c);	//【打印字符对应ASCII码】	
0.6键盘录入 基本类型，首位是0，会自动去除：010->10	直接输出010==默认8进制
0.7:集合.Remove===i--（索引自减）|||StringBuilder 用reverse=需要转回 。toString()	
0.8:int num=0;//变量需要在哪层输出，就定义在哪层(什么位置)。
0.9：***未保存类，提示类中方法未定义
1：if 1可以不接else 2{else}错 

1.0:主函数不对，运行时程序会自动去查找其它同包中的类

1.1:没有保存类==编译没有错，但运行提示：没有加载主类（.java大小为0，编译后未生成.class文件

）

1.2:main错写成mian\\在类中找不到main方法

1.3：改变编码格式，再粘贴编码||编码GBK不可映射字符（notepad\新建\保存\java source.file引起

的）\\\赋值重新建立一个源文件，粘贴

1.4:转义字符格式System.out.print(i+"\t");   \\或“\n”

1.5:循环 最后一次数值判断：1输出每次改变对应结果；2找对应关系：最终“要告知结果”与“判断变

量值”两者关系【】
for(double i=1;【i】<8848;i*=2){
			num++;
		}
		System.out.println("折叠"+【num】+"次，可以折成珠穆朗玛峰的高度");
//i=1 不 num=0 |i=1 满 num=1 i=2 |

1.6:while循环：初始值定义在循环外，所以可以被调用||for不可以

1.7：*1.0==那么整数相除得到小数（即让浮点数参与运算）
	

1.8：int a=10;int b=20;  System.out.print（a=b）;||输出20（即把b的值赋值给a，再输出a）

1.9:利用两个数值交换来：比较循环传入的数
System.out.println("第"+(i+1)+"组平均分为: "+average);
				if(average>init){
					temp=average;
					average=init;
					init=temp;
				}
	}
System.out.println("班级中单组最高平均分为:"+init);


2.0：注意变量，是否写正确--一直变
		 int j;//用于存储商
			int s=0;//存储步数
			do{
				【j】=(num/10);
				s++;
		}while(【j】!=0);

2.1：注意看编译运行的程序是：当前要运行的否  ||防止其它程序干扰
2.2:二维数组传入错误，应该是：数组类型+数组名：String[][] stroeArray

2.3:
switch(meanShow())
return new Scanner(System.in).nextInt();

2.4:char初始化值是：空，但会占位置（"\u0000"）
2.5:setName（"s"）不能放在输出语句
2.6：多个数字输入：采用循环+数组存储，，遍历索引来调用数据
2.7：//不需要导包，编译没问题，但运行会提示找不到文件或无法加载主类
2.8:确定循环次数用for;不确定while;
2.9:break:循环中=结束循环，Switch中=结束循环，Switch；
3.0：数组在内存中【开辟的是连续的空间】：确定数据类型和长度；
3.1:Scanner 类：nextLine():可以接受回车（接收后回车=换行）和空格|||它的前面不能使用其它

Scanner.键盘录入方法[可以有nextLine]
	b:和next()相反
3.2：String s=new String("SS");==创建了两个对象，一个在堆，一个在常量池
3.3：常量池的字符串永远不会变。String s1="ss123";String s2=s1; s2="123";syso(s1)=ss123（不

会改变）
写在同一个方法的字符串，==其值为true,,若在其它对象中，常量池可能不同=地址值不同
3.4:字符串本质是字符串数组
3.5:print：字符数组，可以直接输出（print（char []x））,和字符串一样，有专门的方法；
3.6：split.分割：最后的找到字符切为没||首字符的切割后会有空字符产生。
3.7:方法：引用类型，形参的改变会改变实际值，所以不需要返回值（集合、数组）
3.8:\r\n占两个字符
3.9:alt+shift+a  全局改变量
4.0:FileWirter =new FileWirter("a.txt")===一运行就会覆盖a.txt内容。。。可以换位置，增加中间

变量

4.0：引用数据类型在数组存储的是地址值，二维数组int[3][]:存储的是一维数组地址值
4.1:成员变量为数组，直接在main输出：null
2：名字多了空格
3：不要复制其它地方内容
4：增加public 类（没主函数），，需要另起一栏
5：名称同名，，导致走错方法
6：找不到类，加载不了主函数：类名不对
7:返回值：是调用方法生效
8: 递归算法没有把第一个数考虑进去，报错递归项：“程序执行到底”的时候，会逐层返回
9: 忘记主函数
10：两条语句，注意用{  }，，if{}
11:this应用，注意定义变量名，和调用属性。【‘int’ age = 1;age=7;】
12:public String getID(String ID)：错误
13: 类（）｛}错误，没有（）：cannot be resolved or is not a field
14:随机数：nextInt(100)==0到99
15：有问题，修改好需要:运行一遍
16:System.out.println("test");:先输出test,再换行
17:运算优先顺序；正负、自增减、乘除余、、移位、比较、逻辑运算、、条件、赋值
18：【i<=s.length】：Exception in thread "main" java.lang.ArrayIndexOutOfBoundsException: 3

19：i++ 有中间缓存变量, i = i++ 等价于    【i++是 执行完当前语句才自增；或if(i++)也算语句｛

循环体｝】
temp = i;
i = i + 1;
i = temp;
20:public static void main(String[] args) {
		int m=12;int x=1;int y=2;int s=0;//变量需要赋值必须定义为成员变量
		for(int z=3;z<=m;z++)
			if(m==1)
				System.out.println(0);
			if(m==2)
				System.out.println(1);
			if(m>=3)
			{s=x+y;
		x=y;
		y=s;
	}
21:循环语句：默认下一条语句为循环体=｛循环体｝
    for(int i=1;i<10;i++)  
	System.out.println(i);=执行9次
22：System.out.println( “”+‘a’+1);= a1
23:else--if语句 ，只要一个if为真,其它条件都不执行，都为假执行else
24:	boolean b=true;
		if(b=false)
		{System.out.println("a");}
		System.out.println(b);//结果b=false;【注意‘=赋值’‘==才是比较’】
25：标识符：自己取的名字=不能数字开头，由52个字母，加数字，和_与$
26:构造方法：new的时候执行。类中必须有构造方法，没有javac自动添加		
27:1.static 不能修饰局部变量，，2.局部变量需要初始化，3.静态
方法需调用静态全局变量
【java中成员变量和局部变量的区别
	1.成员变量可以被public，protect，private，static等修饰符修饰，而局部变量不能被控制	

修饰符及static修饰；两者都可以定义成final型
	2.成员变量存储在堆，局部变量存储在栈
	3.存在时间不同
	4.成员变量有默认值，（被final修饰且没有static的必须显式赋值），局部变量不会自动赋值

】
28:继承静态的方法，多态父类调用是子类方法，非静态是父类本身【1.当子父类中，出现同名成员变量

时，多态调用时，只看左边就好，左边是FU，就找父      左边是zi，就找子

	2.出现一模一样的函数时，多态调用，编译时，看的是引用变量所属的类中的方法。运行时，

看的是对象所属的类中的方法。         简单来说：编译看左边，运行看右边

	3.静态函数：静态方法跟类没有关系   只属于类。父类调用，就找父。  简单说 ：编译运行

看左边】
29：局部内部类只能访问被final修饰的变量
30:同一个类中，静态成员只能访问静态成员
31:Scanner接收，如果放在循环里，Scanner一直处于待命状态：if ( arr[idenx]== sc.nextInt())【

语句处于待命状态，输入后再执行。即索引随输入次数递增，再与当时的输入数比较】

32：三元运算符必须要有结果，即返回值; String s= (j==arr2.length-1)?"}":",";
			  System.out.print(s);
或者：System.out.print((j==arr2.length-1)?"}":",");

33:集合.索引.方法可以，用
34:c:System.out.println("涨后工资"+(pay+200)+"元");  用括号调高有限顺序
35:
抽象类
1：没有方法主体｛｝·不允许实例化·只是说明，没有具体
static 方法 可以（不属于多态）=属于整个类不是对象
2：public abstract前缀
3：需要定义子类继承，重写父类抽象的方法，即加主体

36:b:编程规范：1.包名&全小写 2.类名&首字母大写 3.变量与函数名&第一个单词首字母小写，后面单

词首字母大写  4.常量名&都大写_隔开
37：重写必须满足重载要求，即返回值类型也必须一样
38：外部类：不能使用static
39:内部类访问成员变量：其成员变量需要final才能访问到
40：子类继承父类，父类的方法可以直接用
41：把修改的地方标出来：修改1-9..每个修改的地方标出序号
42：正则表达式：
		【()\\1】：两个相同的字符       
		【()\\1{3}】：4个相同的字符
		【([0-9]|10|大?)】:0~9或10，大?，中一个

43：java环境变量配置：jre与jdk分开文件放---cmd>java通过，javac不通过
44：Jdk版本更换,Eclipse需要设置：
	1Properties\Java Build Path\libraries\Jre system libray \remove\add library\对应版

本
 	2Project facets\java\对应版本
45：//注意类名不能于java提供的类名一致，否则调取其方法调用不了
46:运行快捷打开程序:配置环境变量:可以加快捷方式--->不能有空格
47:执行SQL语句:设置同一个值,(0设置成0),
	1.SQLyog提示:0行受影响(没有修改值)
	2.Eclipse返回值=1行受影响(0修改成0)
UPDATE product SET discount=0 WHERE stock<50;  

48:JS中正则和JAVA略有不同
if(/^\s*$/.test(usernameVal))=匹配是否为完全空白,和空数据
	*表示:0到多次===其中0次 :匹配输入框未填数据

usernameVal.match("\\s*")=匹配0至多个空白===什么情况都不满足

eclipse快捷键
ctrl+T:所有实现类   ctrl+o:实现方法 ctrl+shift+r:查找类   ctrl+shift+r:查找文件
alt+shift+z:try catch

49:// 方法提取:不确定返回值=下面语句使用了提取方法定义的变量,或结果.变量名不同不能提取到方

法中

但可以提前到最前面,共用传入参数
//char[] p1copyA = p1copy.toCharArray();// 把字符串转换成字符数组
char[] p1copyR = p1copy.toCharArray();// 复位用
char[] p2copyA = p2copy.toChar..Array();// 把字符串转换成字符数组
char[] p2copyR = p2copy.toCharArray();// 复位用



50:web编码:workspace|web/css|jsp编码
project=clean tomcat=clean------>清除缓冲
复制项目=web project setting; 

51:引用类型,做更改,直接拿去更改就行,不需要赋值回去..不能创建新的.传入.否则指向不对
52:1248----》任何两3个数相加不等于第三4个数，可以表示最大数（x2-1）之间所有数

53：提示情况：需要详细。-->一个个条件判断

54：修改servlet（aday38.jsp）中请求的数据，需要在运行情况下，点击project目录下的clean。等待

console显示:Reloading Context with name [/aday38jsp] is completed，再刷新，才显示结果。（关

闭服务器清除无效）

55：没有导入jar包：commons-logging-1.1.1、在通过反射，执行 BeanUtils封装表单数据方法时，引

起下列异常发生	
	java.lang.reflect.InvocationTargetException
	Caused by: java.lang.NoClassDefFoundError: org/apache/commons/logging/LogFactory
	Caused by: java.lang.ClassNotFoundException: org.apache.commons.logging.LogFactory
56：1.复制粘贴web项目:需要修改properties/web project setting/content root:发布项目名（不然

还是以前的）
2.也会加载两次

57：
1.修改文件前：先复制文件，命名为【原文件名_日期】
2.解决问题时：把百度教程网址保存下来，再修改=记录自己修改了哪些文件
3.或者直接把报错信息，及修改代码复制出来


817：解决在线移除mysql -->yum remove mysql.... 
http://blog.csdn.net/kongdavid/article/details/38313613
http://blog.csdn.net/houjixin/article/details/12653437



tomcat问题:

-bash: ./startup.sh: 权限不够
解决方法：修改权限
[root@localhost bin]# chmod u+x *.sh

[root@localhost bin]# ./startup.sh  
touch: 无法创建"/usr/src/local/tomcat/apache-tomcat-7.0.52-src/logs/catalina.out": 没有那个

文件或目录

解决方法：创建对应目录
mkdir /usr/src/local/tomcat/apache-tomcat-7.0.52-src/logs/

58：static不能和junit共存  单元测试类中不能有static

59:/src/log4j.perproties:没导入,会弹出空指针异常

<--------------------------------------------2:黑马初期笔记-----------------------------

<------------------------------------------------------------------------->
day5.24
快捷键
Shift+右键：打开文件dos命令窗口快捷键
(选项栏会多两行:1在新进程中打开,2在此处打开命令窗口)
cd/：退到根目录
alt+shift+m:循环->方法名

关键字：全部小写，被java赋予特殊含义的字
标识符：用来给包、类、方法、变量等起名字的符号
组成规则：
1unicode:数字，字母，汉字（不建议使用），及其它国家语言（unicode收集的）
2下划线_
3美元符$
注意：1数字不能开头；2不能是java的关键字

注释：描述代码
1单行注释\\
2多行注释/**/
3文档注释/**  */

常量：在程序运行过程中，其值不可以改变
1字符串常量：“hellowrld”
2整数常量
3小数常量
4字符常量
5布尔常量
6空指针常量


变量：其值在程序执行过程中，其值在一定范围内可以发生改变的值
格式： 数据类型 变量名=初始化值

最小信息单元：b；最小存储单元：B=8b

数据类型：基本数据类型+引用数据类型
基本数据类型：
1整数型：byte1 short2 int4 long8  默认int   long后缀 :L
2浮点型:float4 double8 默认double 	    float后缀:F
3字符型:char2
4布尔型:boolean1

命名规则：见名知意
包：字母小写，多个用.隔开
类：每个单词首字母大写
变量、方法：第一个单词首字母小写，后面大写
常量：都大写

osi:开放系统网络连接参考模型:
	物理层、数据链路层、网络层、传输层、会话层、表示层、应用层
通信：应（+包装自己信息）-->表（+信息）--。。-->物理层（+信息）————物理层（解封物理层信

息）-->数据链路层（解析）-->。。-->应用层

字符串拼接：StringBuffer:多线程安全，速度没StringBuilder快

路径：（"//"）=("\"):工具类会自动解析

<--------------------------------------------end:思考-----------------------------

<------------------------------------------------------------------------->
闰年：四年一闰，百年不闰，四百年再闰
思考基础性问题：
1：
	【1.1需确定带符号与不带符号性质】
	a:正数的反码，补码【表现形式相同】，反码（负数）：符号位不变，其它位取反（中间过程

量
	【1.2.计算机没有-0】补码没有正0与负0之分//所以规定1000 0000（为-128补码）
	【1.3.计算机带符号数字都是补码参与运算（反码+1）】
	补码引入的作用是：将减法运算变成加法运算。得出的【结果也为补码】（最高位进位自动溢

出）
	【减法变加法】：时钟12点=0点（即-9 = +3），如果数>12取模%12

	
2：数据结构，算法
	2.1：数据的压缩=找规律|找相同元素|稀疏矩阵思想（把不同值的位置记录好，其它值解压直

接填充）
3：网络层次，丢包

4:汇编语言直接对机器操作：被其解释器转换成二进制码，一条指令对应细微的机器原操作。
不能跨平台（不依赖于操作系统，不依赖与硬件）
原因：操作系统不同；不同的硬件，cpu的指令寄存器不同，x86面向操作系统的

5:Object类与接口关系:Object 与接口采用了同一套方法定义签名---->接口只是知道Object这个类及其

功能,,并拥有
	collection  最上层接口 是iterable(iterator-->foreach功能)
	
趣味思考题：
	1赫夫曼树=最优二叉树；从所有权重点（F集合）里选取两个最小，组成一颗二叉树，
从F中删除两选取权重点，并把其根节点（权重为两选取点之和）作为新的权重点，
加入到F中，直至一棵树

	2四皇后=递归思想：
假设前三个皇后位置都是满足要求的（横、竖，对角不能同时存在两个皇后棋子）
判断最后一个点加入位置是否满足；满足输出，不满足删除当前位置，换位置再判断
	3：汉诺塔
	4：迷宫
	5：九宫格
	6：经典游戏：吃豆人，50层魔塔,推箱子，兔子吃萝卜

<--------------------------------------------3.centos问题解决----------------------------

<------------------------------------------------------------------------->
1.修改文件前：先复制文件，命名为【原文件名_日期】
2.解决问题时：把百度教程网址保存下来，再修改=记录自己修改了哪些文件
3.或者直接把报错信息，及修改代码复制出来


817：解决在线移除mysql -->yum remove mysql.... 
http://blog.csdn.net/kongdavid/article/details/38313613
http://blog.csdn.net/houjixin/article/details/12653437



tomcat问题:

-bash: ./startup.sh: 权限不够
解决方法：修改权限
[root@localhost bin]# chmod u+x *.sh

[root@localhost bin]# ./startup.sh  
touch: 无法创建"/usr/src/local/tomcat/apache-tomcat-7.0.52-src/logs/catalina.out": 没有那个

文件或目录

解决方法：创建对应目录
mkdir /usr/src/local/tomcat/apache-tomcat-7.0.52-src/logs/

-------------------------------------Hibernate--------------------------------------------
60:类全路径名不对:1没有导包;2map时路径不对,不是/////写成了全路径名   3或者字段名对不上 
	org.hibernate.MappingException: class Linkman not found while looking for property: 

lkm_id
	Caused by: org.hibernate.boot.registry.classloading.spi.ClassLoadingException: 

Unable to load class [Linkman]

61:xml等配置文件,`,`表示必须按顺序来配置.  顺序也很重要


62:方法名,类名,包名可能和java工程  的默认名  相同,而覆盖效果

63:sql语句执行时(F9执行),前面的语句也要注意不能有错误.
	
	注意sql中`赋值为0`和`默认为NULL`含义不一样
	
	eg:找出奖金少于100或者没有获得奖金的员工的信息。

SELECT * FROM emp WHERE comm<100 OR comm IS NULL;
sql条件的 :奖金<100  不包含 没有奖金的情况(NULL不小于100)

63:取别名,结果作为值参与运算

64:xml文件修改:
	2.字符串长度也要注意,格式需要匹配
	3.查找时注意取消勾选的选项:通配符 啥的
	4.符号,字符串中是否有符号:< > ! @ & % $　# 等特殊符号
	4.1采用-->格式替换成:!文2字w   特殊不太可能出现的字符串,  然后排查有没有 标签字符等

干扰结果的字符(>  -- 重复格式等)

65:增加辅助列|或替换法进行排序

66:修改mysql密码:
	D:\MYsql\bin
mysqld -nt --skip-grant-tables
use mysql;
update user set password=password("root") where user="root" and host="localhost";
flush privileges;//不刷新==没密码
\q


67:SVN_Url:https://admin-PC:8443/svn/SVN_Reposistory915

68:oracle:解锁账户,修改密码
alter user hr account unlock;
alter user hr identified by (密码);

69:oracle:导入:需要先创建用户
C:\Documents and Settings\Administrator>imp system/oracle file='C:\Documents and
 Settings\Administrator\EXPDAT.DMP' full=y


69:%ShortCut%;%JAVA_HOME%\bin;C:\Program Files (x86)\AMD APP\bin\x86_64;C:\Program Files 

(x86)\AMD APP\bin\x86;%SystemRoot%\system32;%SystemRoot%;%SystemRoot%\System32\Wbem;

%SYSTEMROOT%\System32\WindowsPowerShell\v1.0\;C:\Program Files (x86)\ATI Technologies

\ATI.ACE\Core-Static;D:\MYsql\bin;C:\Program Files (x86)\Intel\OpenCL SDK\2.0\bin\x86;C:

\Program Files (x86)\Intel\OpenCL SDK\2.0\bin\x64;C:\Program Files (x86)\Intel\OpenCL SDK

\2.0\bin\x86;C:\Program Files (x86)\Intel\OpenCL SDK\2.0\bin\x64;D:\VisualSVN\bin;D:

\TortoiseSVN\bin


70:注意 每个 可以 点击 的地方

36220119930521343x
362201199308223414

71:oracle 连接不上 oracle is not aviable
需要重启服务器:oracle..listen oracleService

维基百科
wiki12306
wikizhishi

72:重复利用搜索(设置搜索条件:搜索内容) 定位需要查找的内容位置:  windows关键字搜索:可以搜索

到老师敲的源代码里面的内容

73:更新项目,文件出现感叹号,pom文件导包失败,联网导包
--->需要找到提示未找到的jar,,对应的本地仓库,删除器不完整的jar等文件,然后,更新项目-->联网重

新下载

74:在项目下创建包,结果却是以文件夹结构生成.
--->右键/build path/configure Build Path /jre system Library  /改成eclipse默认的jre

75:WebService生成客户:Failed to parse the WSDL.
wsimport -s . http://localhost:22345/user?wsdl-->此ip代表的是本地:不能联网..


76:压栈,数据获取不到------>压栈和获取的页面不一样

77:页面内容,,打开项目目录,通过windows内容查找,定位对应操作指定页面选项的类,,,,例如:名称空间

NameSpace(/cargo)路径:*NameSpace*cargo) --->定位到操作 货运管理 的   或

shippingOrderAction_list

78:下载文件:可以页面查找--->zip
删除:刷新--->时间戳不是最新的
逆向工程:重复生成会产生特殊不可见字符,编译会出问题,-->先删除在生成


79:mybatis sql注入问题
	name=王二麻子
	#{}预处理 使用PrepareStatement ,变量出用 ? 代替,将传入的参数当成字符串解析后 加上引

号"",有效防止sql注入
	${}为原样输出 ,需要传入数据库字段-->动态排序需要用,可以自己预先指定,或者对值进行判

断//不进行用户输入
:openSession.selectList("user.findUserByName"," 1 or 1=1");
#{value}
SELECT `userId`,`name`,`age` FROM `user` where name like "1 or 1=1"
${value}
SELECT `userId`,`name`,`age` FROM `user` where name like 1 or 1=1 


	例如:传入值openSession.selectList("user.findUserByName","name");   传入值为字符串,
SELECT * FROM `user` WHERE order by  ${value} ----->一个值只能用  value

#{}替换掉${}
Oracle数据库
select * from USER_P where user_name like '%'||#{name}||'%';
MySQL数据库
SELECT * FROM`user` WHERE `name` LIKE CONCAT('%',#{name},'%')


SELECT * FROM `user` WHERE age like '%${age}%' and  name like '%${name}%'

SELECT * FROM`user` WHERE `name` LIKE '' OR 1=1   OR '';and id=1001;-->可以拼接其它条件




79:记得自己的操作步骤:可能的误操作,startup.sh    --->启动了linus服务l....而不是startup.bat



80:<fieldType name="text_ik" class="solr.TextField" >
xml配置时:注意字段和"引号" 的间距
]


81:子类继承父类:创建子类对象时,发现extends关键子,会先加载父类对象

开始:Zi zi = new Zi();
------------------------------静态代码块区1---------------
步骤:1.父类-静态初始化-变量:2次
2.父类-静态初始化-代码块:1:syso 2:}

3.子类---静态初始化-变量
4.子类-静态初始化-代码块
---------------------------------构造器super()1.1------------------
----Zi zi = new Zi();----
5.子类:super()
6.父类:super()

------------------------------常量,代码块区2------------
7.父类-变量
8.父类-代码块
-------------------------------构造器等级2.1----------
9.父类构造器


10.子类-变量
11.子类-代码块
12.子类-构造器
----Zi zi2 = new Zi();----
13.
5.6.7.8.9.10.11.12




80:注意edit.plus编辑后添加了***.bak文件,以及修改xml文件时可能影响

81:Together_1024

82:   显示git图标
  3.打开regedit.exe，准备修改注册表

    找到 HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Explorer

    新建一个“字符串值”名称为 “Max Cached Icons” 值是 “2000”

重启一下电脑，图标就显示了。

83:telnet 192.168.131.73 1521-->1测试端口有没有开放
开放：则会跳转显示黑框
没开放：2.对方Listen服务没有打开：重启服务（oracle....listen...）
1.说明对方主机没有开（ping 测试）
