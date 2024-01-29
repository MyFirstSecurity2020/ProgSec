# Linux C 程式設計_part 1:範例學習(本次課程)
- [20240128第一次教學錄影](https://youtu.be/EPMsu_SoLPE)
- [20240128第二次教學錄影](https://youtu.be/BFYjyARU9Ec)
- 格式化輸入與輸出|運算
  - 輸入與輸出:printf()與scanf()
  - 各種運算:
    - 算術運算子（Arithmetic Operators）: 加減乘除
    - 遞增和遞減運算字（Increment and Decrement Operators）: ++y  x--
    - 關係運算子（Relational Operators）: > >= ...
    - 邏輯運算子（Logical Operators）: and | or | xor
    - 位元運算子(Bitwise operators)
  - 運算子的優先順序:先乘除 後加減
- 流程控制:
- 迴圈設計1(loop_1):for 迴圈|while 迴圈| do ⋯ while 迴圈|
- 迴圈設計2(loop_2):break 敘述| continue 敘述|多重迴圈
- 函數
  - 函數呼叫:call by value(傳值呼叫) vs call by address(傳址呼叫)
  - 遞迴函數
  - 變數類型與scope(管轄範圍)
- 陣列(同質性資料)
- 字串
# Linux C 程式設計_part 2:(下次課程 | 錄影教學)
- 指標變數(pointer)
  - `*` 與 &運算
  - 指標變數的加法運算與減法運算 
- 使用指標變數存取陣列
- 使用指標變數字串
- 結構體(異質性資料)
- 動態記憶體配置

# 參考書
- [C 語言教學手冊, 4/e](https://www.tenlong.com.tw/products/9789574424849?list_name=srh)
- C語言程序設計 : 現代方法, 2/e (修訂版) C Programming: A Modern Approach, 2/e
  - [英文版](https://www.tenlong.com.tw/products/9780393979503?list_name=srh)
  - [簡體中譯本](https://www.tenlong.com.tw/products/9787115565198?list_name=srh) 
- 線上學習資源
  - https://www.runoob.com/cprogramming/c-tutorial.html
  - https://www.geeksforgeeks.org/c-programming-language/?ref=shm   
- https://en.wikipedia.org/wiki/C_(programming_language)
# 開發環境
- online C compiler
  - https://www.onlinegdb.com/online_c_compiler
- Linux 
  - gcc(c) | g++(c++)
  - GNU Compiler Collection (GCC)
  - [GCC online documentation](https://gcc.gnu.org/onlinedocs/)
- Windows
  - dev-c++
    - https://www.bloodshed.net/ 
  - visual studio code
    - https://code.visualstudio.com/ 

### 範例1:輸入與輸出
```c
#include <stdio.h>

int main(void) {
	float miles;

	printf("Please enter miles:");
	scanf("%f", &miles);

	float kilometers = miles * 1.6;

	printf("%f Kilometers", kilometers);
}
```
- 編譯: gcc ex1.c -o ex1
- 執行: ./ex1
```c
#include <stdio.h>

int main(void) {
	float miles,kilometers;

	printf("Please enter miles:");
	scanf("%f", &miles);

	kilometers = miles * 1.6;

	printf("%f Kilometers", kilometers);
}
```
## 格式化輸出
```
%c：以字元方式輸出

%d：10 進位整數輸出
%o：以 8 進位整數方式輸出
%x、%X：將整數以 16 進位方式輸出

%u：無號整數輸出
%lu：long unsigned 型態的整數

%f：浮點數輸出
%e、%E：使用科學記號顯示浮點數
%g、%G：浮點數輸出，取 %f 或 %e（%f 或 %E），看哪個表示精簡
%%：顯示 %

%s：字串輸出
%p：指標型態 
```
### 範例2:ASCII 編碼與解碼   https://zh.wikipedia.org/wiki/ASCII
```
#include <stdio.h>

int main(void) {
    printf("ASCII 編碼與解碼 初初階\n");
    printf("顯示字元 %c\n", 'A');
    printf("顯示為十進位整數 %d\n", 'A');
    printf("顯示為八進位整數 %o\n", 'A');
    printf("顯示為十六進位整數 %X\n", 'A');
    printf("顯示為十六進位整數 %x\n", 'A');
    
    return 0;
}
```
### 範例3:格式化輸入與輸出 | 算術運算子（Arithmetic Operators）
```c
#include <stdio.h>
#include <math.h> 

int main()
{
   float a = 1.0, b = 6.0, c=4.0;
   printf ("%.4f", sqrt(a+b*c));
   return 0;
}
```
- 程式編譯
  - gcc xxx.c -lm
  - https://stackoverflow.com/questions/10409032/why-am-i-getting-undefined-reference-to-sqrt-error-even-though-i-include-math
- sqrt()函數是定義在<math.h> ==> 所以必須要#include <math.h> 
- 更多數學運算範例請參看
  - https://blog.hubspot.com/website/math-functions-c
  - https://www.w3schools.com/c/c_math.php


### 範例4:bitwise運算子（Logical Operators）
```c
#include <stdio.h>
int main(int argc, char **argv)
{
    int x=9;
    int y=5;
    int result=(x^y);
    int result2=(x&&y);
    int result3=(x&y);
    printf("this is the smallest number %d \n", result);
    return 0;
}
```
```c
#include <stdio.h>
int main(int argc, char **argv)
{
    int x=9;
    int y=5;
    int result=y^((x^y)&-(x<y));
    printf("this is the smallest number %d \n", result);
    return 0;
}
```

### 範例5: 遞增和遞減運算字（Increment and Decrement Operators）
```c
#include <stdio.h>
int main()
{
   int a = 11111, b = 22222;
   printf("%d", (a++)+(++b));
   return 0;
}
```

```c
#include <stdio.h>
int main()
{
   int a = 11111, b = 22222;
   printf("%d", (a++)+(a+(++b)));
   return 0;
}
```
# 選擇性敘述 ==> 各類型 if   switch
## 範例6: if
```
#include<stdio.h>
 
int main()
{
    int num;
 
    printf("請輸入一個正整數 : ");
    scanf("%d",&num);
 
    if (num%2==0)
      printf("你輸入的偶數");
}
```
## 範例7: if ..else ..
```
#include<stdio.h>
 
int main()
{
    int num;
 
    printf("請輸入一個正整數 : ");
    scanf("%d",&num);
 
    if (num%2==0)
      printf("你輸入的偶數\n");
    else
      printf("你輸入的奇數\n");
}
```
## 範例8: `? : `運算子(三元運算子)
```
#include<stdio.h>
 
int main()
{
    int num;
 
    printf("請輸入一個正整數 : ");
    scanf("%d",&num);
 
    (num%2==0)?printf("偶數"):printf("奇數");
}
```
### 範例9: if-else流程控制
```
試寫一個C程式，能判定輸入年份是否為閏年(leap year) 。
閏年判定方式：是4的倍數，但不是100的倍數：或者是400的倍數
　　例如：1800閏年，2000是閏年，2001不是閏年
```
```c
#include <stdio.h>
int main()
{
   int year;
   printf("判斷是否為閏年的C程式:請輸入你要的......年份"); 
   scanf("%d",&year);	

   if(((year%4==0)&&(year%100!=0))||(year%400==0))
       printf("%d 年是閏年.",year);
   else
       printf("%d 年不是閏年r",year);    

   return 0;
 }
```

### 範例10: switch流程控制
```c
#include <stdio.h>

int main()
{
   int x = 3;
   switch (x+1) {
     case 3:
       printf ("3  ");
     case 4:
       printf ("4  ");
     case 5:
       printf ("5  ");
       break;
     case 6:
       printf ("6  ");
     default:
       printf ("x");
     }
   return 0;
}
```
# 迴圈設計
### 範例11:迴圈設計
- 題目:在console端輸入n == > 輸出:1+2+3+….+n的結果
- 使用三種loop技術撰寫
```c
//FOR LOOP

#include <stdio.h>
int main() {
    int n, i, sum = 0;

    printf("Enter a positive integer: ");
    scanf("%d", &n);

    for (i = 1; i <= n; ++i) {
        sum += i;  // sum = sum +i
    }

    printf("Sum = %d", sum);
    return 0;
}


```
```c
//while loop

#include <stdio.h>
int main() {
    int n, i, sum = 0;

    printf("Enter a positive integer: ");
    scanf("%d", &n);

    i = 1;
    while (i <= n) {
       sum += i;
       ++i;
    }


    printf("Sum = %d", sum);
    return 0;
}


```
```c
//DO While LOOP

#include <stdio.h>
int main() {
    int n, i, sum = 0;

    printf("Enter a positive integer: ");
    scanf("%d", &n);

    i = 1;
    do{
      sum += i;
      ++i;
    } while (i <= n);

    printf("Sum = %d", sum);
    return 0;
}
```
- 練習作業:在console端輸入n == > 輸出:n!=1*2*3*….*n的結果
  - 使用三種loop技術撰寫
  - 3!=3*2*1 =6
- 練習作業:底下輸出結果是多少? and why?
```c
#include <stdio.h>
#include <stdlib.h>
int main(void) {
  int x;
  float y;
  for (x=0, y=50; x<25; x+=5, y/=2)
    printf("x=%d, y=%4.2f\n", x, y);
  return 0;
}
```
x=20, y=3.12


### 範例12:多重迴圈範例: 99乘法表
```c
#include <stdio.h>
int main() {
    int i,j;   
    for(i=1;i<=9;i++) {
        for(j=1;j<=9;j++)
            printf("%d*%d=%2d\t", i, j, i*j);
        printf("\n");
    }
    return 0;
}
```

- 練習作業:底下輸出結果是多少? and why?
```c
#include <stdio.h>
#include <stdlib.h>

int main(int argc, char* argv[])
{
   int i, sum = 2, prm = atoi(argv[1]);
   for(i = 3; i < prm; i++)
   {
      int j;
      int flag = 1;
      for(j = i - 1; j > 1; j--)
      {
         if(i % j == 0)
         {
            flag = 0;
            break;
         }
      }

      if(flag == 1)
         sum += i;
         
   }
   printf("The sum is: %d\n", sum);
}
```
- atoi()-將字串轉換成整數

- 練習作業:底下輸出結果是多少? and why?
```c
#include <stdio.h>

int main(int argc, char *argv[])
{
   int i, sum = 0;
   for(i = 0; i < 100; i++)
   {
      if(i % 3 == 0 && i % 2 == 0)
         sum += i;
   }
   printf("The sum is: %d\n", sum);
   return 0;
}
```

- 練習作業:底下輸出結果是多少? and why?
```c
#include<stdio.h>
void main(void){
   int k=0, total=0;
   while(k<=16){
     if(k % 4 != 0){
       k++;
       continue;
     }
    
     total +=k;
     k++;
     }

   printf("Total=%d\n", total);
}
```
# 函數
### 範例13:函數(Function)
- main()在後 其他函數在前
```
#include <stdio.h>
 
int ifactorial(int z)
{
	int mul = 1, i = 1;
	while(i <= z)
	{
		mul *= i;
		i++;
	};
	return mul;
}

int  main()
{
    int i = 4;
    printf("%d 的階乘為%d\n", i, ifactorial(i));
    return 0;
}
```
- main()在前 其他函數在後
```c
#include <stdio.h>
#include <stdlib.h>

int a=10, fun(int);

int main(void) {

  int b=6;
  printf("a=%d, b=%d, fun(a)=%d\n", a, b, fun(a));
  return 0;
}

int fun(int b) {
  a -=5; b /=2;
  return(a+b);
}
```
a=5, b=6, fun(a)=10

### 範例14: 函數呼叫:call by `value`(傳`值`呼叫) vs call by `address`(傳`址`呼叫)| 兩個數字互換的C程式
```c
#include <stdio.h>
/* 函數的宣告 */
void swap (int a, int b);

int main (void) {
  int i = 11, j = 22;
  printf ("i = %d, j = %d\n" , i, j);
  swap (i, j);
  printf ("i = %d, j = %d\n" , i, j);
  return 0;
}

void swap (int a, int b) {
  printf ("互換前:a = %d, b = %d\n" , a, b);
  int temp = a;
  a = b;
  b = temp;
  printf ("互換後:a = %d, b = %d\n" , a, b);
}
```
## 遞迴函數
## 範例15:遞迴函數:計算n!
- 遞迴式:f(n) = n*(n-1)*(n-2)*......1 = n*f(n-1)
-        f(3)=3*f(2)=3*[2*f(1)]=3*[2*{1}]
- 終止式:f(1)=1
```
#include <stdio.h>
 
double factorial(unsigned int i)
{
   if(i <= 1)
      return 1;
   else   return i * factorial(i - 1);
}

int  main()
{
    int i = 15;
    printf("%d 的階乘為%f\n", i, factorial(i));
    return 0;
}
```

### 範例16:費式序列Fibonacci Serie
- 費式序列Fibonacci Series: 0 1 1 2 3 5 8 13 21 34
- f(0)=0, f(1)=1, f(n)=f(n-1)+f(n-2)
- 底下是用迴圈方式計算費式序列Fibonacci Serie
- 作業:使用遞迴函數方式計算費式序列Fibonacci Serie
```c
#include<stdio.h>    
void printFibonacci(int n){    
  static int n1=0,n2=1,n3;    

  if(n>0){    
    n3 = n1 + n2;    
    n1 = n2;    
    n2 = n3;    
    printf("%d ",n3);    
    printFibonacci(n-1);    
    }    
 }    

int main(){    
   int n;
  
   printf("請輸入你要列印幾項費式序列(要整數): ");    
   scanf("%d",&n);    
   printf("費式序列Fibonacci Series: ");    
   printf("%d %d ",0,1);//註解1:先列印前兩個費式序列   
   printFibonacci(n-2);//註解2:在印出其他費式序列   
   return 0;  
 }    
```
### 範例17:變數類型與scope(管轄範圍)
```c
#include <stdio.h>
 
/* 全域(global)變數宣告 */
int g = 20;

void printg()
{
  printf ("value of g in printg= %d\n",  g);
}

void printg2()
{
  /* 區域(local)變數宣告 */
  int g = 99;
  printf ("value of g in printg2= %d\n",  g);
}

int main ()
{
  /* 區域變數宣告 */
  int g = 10;

  printg();
  printf ("value of g in main= %d\n",  g);
 
  return 0;
}
```
### 範例18:陣列
- 陣列的存取方式:
  - 1.使用索引(index) 存取陣列資料
  - 2.使用指標(pointer)存取陣列資料
```c
#include <stdio.h>
 
int main ()
{
   int n[10]; /* n 是一個包含 10 個整數的陣列 */
   int i,j;
 
   /* 初始化陣列元素 */         
   for ( i = 0; i < 10; i++ )
   {
      n[ i ] = i + 100; /* 設置元素 i 為 i + 100 */
   }
   
   /* 輸出陣列中每個元素的值 */
   for (j = 0; j < 10; j++ )
   {
      printf("Element[%d] = %d\n", j, n[j] );
   }
 
   return 0;
}

```
### 範例19:字串(==字元陣列)與字串處理(不使用指標)
```c
#include <stdio.h>
#include <string.h>
 
int main ()
{
   char str1[9] = "CTFer";
   char str2[9] = "hacker";
   char str3[9];
   char str4[9];
   int  len ;
 
   /* 複製 str1 的內容複製到 str3 */
   strcpy(str3, str1);
   printf("strcpy( str3, str1) :  %s\n", str3 );
 
   /* 連接 str1 和 str2後的結果 存到str1 */
   strcat( str1, str2);
   printf("strcat( str1, str2):   %s\n", str1 );
 
    /* 連接 str2 和 str1後的結果 存到str1   */
   strcat( str2, str1);
   printf("strcat( str2, str1):   %s\n", str2 );
   
   /* 連接後，str1 的總長度 */
   len = strlen(str1);
   printf("strlen(str1) :  %d\n", len );
 
   strcpy(str4, str1);
   printf("strcpy( str4, str1) :  %s\n", str3 );
   str4[3] = '\0';
   printf(str4);
   
   return 0;
}
```
```
https://www.onlinegdb.com/online_c_compiler 

執行結果
main.c:38:11: warning: format not a string literal and no format arguments [-Wformat-security]    
    printf(str4 );                                                                                
           ^~~~                                                                                   
strcpy( str3, str1) :  CTFer                                                                      
strcat( str1, str2):   CTFerhacker                                                                
strcat( str2, str1):   erCTFerhacker                                                              
strlen(str1) :  22                                                                                
strcpy( str4, str1) :  cker                                                                       
*** stack smashing detected ***: ./a.out terminated                                               
CTFAborted (core dumped)    
```
- 修正後的程式
```
#include <stdio.h>
#include <string.h>
 
int main ()
{
   char str1[9] = "CTFer";
   char str2[9] = "hacker";
   char str3[9];
   char str4[9];
   int  len ;
 
   /* 複製 str1 的內容複製到 str3 與str 4 */
   strcpy(str4, str1);
   strcpy(str3, str1);
   printf("strcpy( str3, str1) :  %s\n", str3 );
 
   /* 連接 str1 和 str2後的結果 存到str1 */
   strcat( str1, str2);
   printf("strcat( str1, str2):   %s\n", str1 );
 
    /* 連接 str2 和 str1後的結果 存到str1   */
   //strcat( str2, str1);
   //printf("strcat( str2, str1):   %s\n", str2 );
   
   /* 連接後，str1 的總長度 */
   len = strlen(str1);
   printf("strlen(str1) :  %d\n", len );
 
   printf("strcpy( str4, str1) :  %s\n", str4 );
   str4[3] = '\0';
   printf("處理過的字串變成(請說明why?) :  %s\n",str4);
   
   return 0;
}
```

