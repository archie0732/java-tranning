# 開始java

1. 基本架構 & 輸出 
```java
public class hello//你建的檔案名
{
  public static void main(String[] args) {//建立主程式(void==>不回傳值)

    //你的程式寫在這裡
    // System.out.println();輸出在括號內的值  !! 注意大小寫!!
     System.out.println("Hello java")//因為是字串所以需要放在" "內

  }
}
```
2. 如何執行程式
```md
 * 編譯與執行  
 * 儲存: ctrl+s
     (在終端機中輸入` `包含之指令)
 * 1. 編譯: `javac 檔名.java` ==> 編譯(檢查有沒有寫錯)，並建一個 檔名.class (沒有也沒差)  
 * 2. 執行: `java 檔名 (不用加.java)` ==> 執行你寫的檔案  
``` 
3. 輸入值  
 >首先，要在程式最上面加入`import java.util.Scanner;`  
 >建立一個物件:`Scanner 變數名稱1 = new Scanner(System.in);`  
 >導入輸入值與宣告型態  
 >  >`int 變數名稱2=變數名稱1.nextlnt()`要導入數字     
 >  >`string 變數名稱2=變數名稱1.next()`導入文字
>   >
 >輸入就存於 **變數名稱2** 裡了 
 
* 範例

數字版
```java
import java.util.Scanner; 
public class javatest
{
  public static void main(String[] args) {
    Scanner s=new Scanner(System.in);// 建立
    System.out.println("請輸入整數")

    //輸入值
    int a=s.nextInt();
    //輸出你輸入的數字乘10的結果
    System.out.println(a*10);

  }
}
```
文字版
```java
import java.util.Scanner; 
public class javatest
{
  public static void main(String[] args) {
    Scanner s=new Scanner(System.in);// 建立
    System.out.println("請輸入你的名字")

    //輸入值
    int a=s.next();
    //輸出你輸入的名字 加上 你好
    System.out.println(a+"你好"); 

  }
}
```

 
