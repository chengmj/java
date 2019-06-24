## java基础
### HelloWorld
- java是区分大小写的
- 类名与文件名要一致，如下示例文件名必须为HelloWorld.java
```
public class HelloWorld {
    public static void main(String[] args){
        System.out.println("Hello World!");
        System.out.println(5+6);
    }
}
```

### java中的字符集
- java中用的是UTF-16编码的Unicode。
- UTF-16用16个bit，即两个byte，这也是char占用两个byte的原因。当把char转成数字的时候，需要用int。
- String不是java中的保留字。

```
public class HelloWorld {
    public static void main(String[] args){
        System.out.println("Hello World!");
        double a = 99;
        int b = 5;
        System.out.println(a/b);
        System.out.println("a + b =" + a + b);   //此处考虑算术运算优先级，+ 为字符串拼接
        System.out.println("a + b =" + (a + b));
        System.out.println("a\tb\n\\n");
        char d = '\u81e7';
        System.out.println(d);
        System.out.println(1==1);
        System.out.println(a < b);
    }
}

```
输出结果：    
```
Hello World!
19.8
a + b =99.05
a + b =104.0
a	b
\n
臧
true
false

```
