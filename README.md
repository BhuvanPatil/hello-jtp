# hello-jtp
P1:
---

class Simple
{  
    public static void main(String args[])
    {  
     System.out.println("Hello Java");  
    }  
}  


P2:
---

class A
{
	public static void main(String args[])
	{
		System.out.println("Welcome to Java Programming...");
	}
}

P3:
---

//Save the entire below code with file name as Hard.java

class B
{
	public  void printB()
	{
		System.out.println("Hi am from B class..");
		
	}
}
class C
{
	public  void printC()
	{
		System.out.println("Hi am from C class..");
		
	}
}
class D
{
	public  void printD()
	{
		System.out.println("Hi am from B class..");
		
	}
}
class Hard
{
	public static void main(String args[])
	{
		B b1 = new B();
		C c1 = new C();
		D d1 = new D();

		b1.printB();
		c1.printC();
		d1.printD();
	}
}

//To Compile: 	C:/>javac -d ../classes Hard.java
//To Execute:   C:/>java -cp ../classes Hard
/* here after Compiling the Hard.java file, the compiler will generate total 4 .class file named as B.class C.class D.class and Hard.class

O/P:
----
Compile:  E:\jdk1.8.0_102\bin\jdk1.8.0_103\src>javac -d ../classes Hard.java
\
Running: E:\jdk1.8.0_102\bin\jdk1.8.0_103\src>java -cp ../classes Hard
Hi am from B class..
Hi am from C class..
Hi am from B class..

*/

/* 
P4:
//Example to understand the types of variables in java
claSS E
{
  int data = 50;
  static int m = 100;
  void method()
  {
	int n = 90;
  }
}	
*/

/*
P5: Java Variable Example: Add Two Numbers
class F
{
	public static void main(String args[])
	{
		int a = 10;
		int b = 20;
		int c = a + b;
		System.out.println("Sum of a & b: "+c);
	}
}
O/P:
----
E:\jdk1.8.0_102\bin\jdk1.8.0_103\src>javac -d ../classes F.java
E:\jdk1.8.0_102\bin\jdk1.8.0_103\src>java -cp ../classes F
Sum of a & b: 30

*/

/*
P6:Java Variable Example: Widening
class G
{
	public static void main(String args[])
	{
		int a = 10;
		float f = a;

		System.out.println("Autowidening of int(a) to float(f): "+f);
	}
}
O/P:
E:\jdk1.8.0_102\bin\jdk1.8.0_103\src>javac -d ../classes G.java
E:\jdk1.8.0_102\bin\jdk1.8.0_103\src>java -cp ../classes G
Autowidening of int(a) to float(f): 10.0

*/
/*
P6:

//Java Variable Example: Narrowing (Typecasting)

class H
{  
	public static void main(String[] args)
	{  
		float f=10.5f;  
		//int a=f;//Compile time error  
		int a=(int)f;  
		System.out.println("f: "+f);  
		System.out.println("a: "+a);  
	}
}  

/*
E:\jdk1.8.0_102\bin\jdk1.8.0_103\src>javac -d ../classes H.java


E:\jdk1.8.0_102\bin\jdk1.8.0_103\src>java -cp ../classes H

f: 10.5
a: 10
*/
/*
P7:
//Java Variable Example: Overflow
class I
{
	public static void main(String args[])
	{
		int a = 130;
		byte b = (byte)a;
		System.out.println("a: "+a);
		System.out.println("b: "+b);
	}
}


O/P:
E:\jdk1.8.0_102\bin\jdk1.8.0_103\src>javac -d ../classes I.java

E:\jdk1.8.0_102\bin\jdk1.8.0_103\src>java -cp ../classes I

a: 130
b: -126

*/

/*
P8:
//Java Variable Example: Adding Lower Type

class J
{
	public static void main(String args[])
	{
		byte a = 10;
		byte b = 10;
		byte c = (byte)(a+b);
		System.out.println("c: "+c);
	}
}
/*
O/\P:

E:\jdk1.8.0_102\bin\jdk1.8.0_103\src>javac -d ../classes J.java

E:\jdk1.8.0_102\bin\jdk1.8.0_103\src>java -cp ../classes J

c: 20

*/
*/
/*
P9:
//Java Unary Operator Example1: ++ and --
class K
{
	public static void main(String args[])
	{
		int a = 10;
		
		System.out.println("a :"+a); //10
		System.out.println("a++ :"+ a++); //10
		System.out.println("a-- :"+ a--); //11
		System.out.println("++a :"+ ++a);//11		
		System.out.println("--a :"+ --a);//10
		System.out.println("a :"+a);//10
	}
}
/*
E:\jdk1.8.0_102\bin\jdk1.8.0_103\src>javac -d ../classes K.java

E:\jdk1.8.0_102\bin\jdk1.8.0_103\src>java -cp ../classes K

a :10
a++ :10
a-- :11
++a :11
--a :10
a :10

*/

*/
/*
P10:
//Java Unary Operator Example 2: ++ and --

class OperatorExample
{  
	public static void main(String args[])
	{  
		int a=10;  
		int b=10;  
		System.out.println(a++ + ++a);//10+12=22  
		System.out.println(b++ + b++);//10+11=21  
	}
} 
*/

/*
P11: Java Unary Operator Example 2: ++ and --
class Testarray
{
	public static void main(String args[])
	{
		int a = 10;
		int b = 10;
		System.out.println(a++ + ++a);
		//                 10     12 = 22
		System.out.println(b++ + ++b);
		//                 10    12   = 22
		System.out.println(b++ + b++);//25
	//                

	}
}
*/

/*
P12: Java Unary Operator Example: ~ and !
//Java Unary Operator Example: ~ and !
class Op1
{
	public static void main(String args[])
	{
		int a = 10;
		int b = -10;
		boolean c = true;
		boolean d = false;
		System.out.println("a: "+ ~a);// -11
		System.out.println("b: "+ ~b);// 9
		System.out.println("!c: "+ !c);// false
		System.out.println("!d: "+ !d);// true
	}
}

/*
O/P:
E:\Software\JDK\jdk-7u17-windows-i586\lib\Operators\src>javac -d ../classes Op1.
java

E:\Software\JDK\jdk-7u17-windows-i586\lib\Operators\src>java -cp ../classes Op1
a: -11
b: 9
!c: false
!d: true

*/

*/

/*
P13:Java Arithmetic Operator Example
class Op2
{
	public static void main(String args[])
	{
		int a = 10;
	    	int b = 5;
		System.out.println(a+b);
		System.out.println(a-b);
		System.out.println(a*b);
		System.out.println(a/b);
		System.out.println(a%b);
	}
}
/*
O/P:
-----
15                                                                                                                             
5                                                                                                                              
50                                                                                                                             
2                                                                                                                              
0   
*/
*/
/*
P14:Java Arithmetic Operator Example: Expression
class Op3
{  
	public static void main(String args[])
	{  
		System.out.println(10*10/5+3-1*4/2);  
	}
}  

/*
O/P:
----
21

*/
*/

/*
P15: Java Left Shift Operator Example
class Op4
{  
	public static void main(String args[])
	{  
		System.out.println(10<<2);//10*2^2=10*4=40  
		System.out.println(10<<3);//10*2^3=10*8=80  
		System.out.println(20<<2);//20*2^2=20*4=80  
		System.out.println(15<<4);//15*2^4=15*16=240  
	}
}  
Output:

40
80
80
240

*/

/*
P16: Java Right Shift Operator Example
//The Java right shift operator >> is used to move left operands value to right by the number of bits specified by the right operand.
class OperatorExample
{  
	public static void main(String args[])
	{  
		System.out.println(10>>2);//10/2^2=10/4=2  
		System.out.println(20>>2);//20/2^2=20/4=5  
		System.out.println(20>>3);//20/2^3=20/8=2  
	}
}  
O/P:
2
5
2

*/
/*
P17: Java Shift Operator Example: >> vs >>>
class OperatorExample
{  
    public static void main(String args[])
    {  
	    //For positive number, >> and >>> works same  
	    System.out.println(20>>2);  
	    System.out.println(20>>>2);  
	    //For negative number, >>> changes parity bit (MSB) to 0  
	    System.out.println(-20>>2);  
	    System.out.println(-20>>>2);  
    }
}  
O/P:
5                                                                                                                              
5                                                                                                                              
-5                                                                                                                             
1073741819 
*/
/*
P18: Java AND Operator Example: Logical && and Bitwise &

class OperatorExample{  
public static void main(String args[]){  
int a=10;  
int b=5;  
int c=20;  
System.out.println(a<b&&a<c);//false && true = false  
System.out.println(a<b&a<c);//false & true = false  
}}  
Output:

false
false

*/
/*
P19: Java AND Operator Example: Logical && vs Bitwise &
class OperatorExample
{  
	public static void main(String args[])
	{  
		int a=10;  
		int b=5;  
		int c=20;  
		System.out.println(a<b&&a++<c);//false && true = false  
		System.out.println(a);//10 because second condition is not checked  
		System.out.println(a<b&a++<c);//false && true = false  
		System.out.println(a);//11 because second condition is checked  
	}
}  
Output:

false
10
false
11

*/

/*
P20: Java OR Operator Example: Logical || and Bitwise |
The logical || operator doesn't check second condition if first condition is true. It checks second condition only if first one is false.

The bitwise | operator always checks both conditions whether first condition is true or false.

class OperatorExample
{  
	public static void main(String args[])
	{  
		int a=10;  
		int b=5;  
		int c=20;  
		System.out.println(a>b||a<c);//true || true = true  
		System.out.println(a>b|a<c);//true | true = true  
		//|| vs |  
		System.out.println(a>b||a++<c);//true || true = true  
		System.out.println(a);//10 because second condition is not checked  
		System.out.println(a>b|a++<c);//true | true = true  
		System.out.println(a);//11 because second condition is checked  
	}
}  
Output:

true
true
true
10
true
11

*/

/*
P21:ava Ternary Operator Example
class OperatorExample
{  
	public static void main(String args[])
	{  
		int a=2;  
		int b=5;  
		int min=(a<b)?a:b;  
		System.out.println("min: "+min);  
	}
}  
Output:

min: 2

*/

/*
P22:
class OperatorExample
{  
	public static void main(String args[])
	{  
		int a=10;  
		int b=5;  
		int min=(a<b)?a:b;  
		System.out.println("min: "+min);  
	}
}  
Output:

5

*/
/*
//Java Assignment Operators
P23:Java Assignment Operator Example
class OperatorExample
{  
	public static void main(String args[])
	{  
		int a=10;  
		int b=20;  
		a += 4;//a=a+4 (a=10+4)  
		b -= 4;//b=b-4 (b=20-4)  
		System.out.println(a);  
		System.out.println(b);  
	}
}  
Output:

14
16
*/
/*
P24: Java Assignment Operator Example
class OperatorExample
{  
	public static void main(String[] args)
	{  
		int a=10;  
		a += 3;//10+3  
		System.out.println(a);  
		a -= 4;//13-4  
		System.out.println(a);  
		a *= 2;//9*2  
		System.out.println(a);  
		a /= 2;//18/2  
		System.out.println(a);  
	}
}  
Output:

13
9
18
9

*/
/*
P25: Java Assignment Operator Example: Adding short
class OperatorExample
{  
	public static void main(String args[])
	{  
	short a=10;  
	short b=10;  
	//a+=b;//a=a+b internally so fine  
	a=a+b;//Compile time error because 10+10=20 now int  
	System.out.println(a);  
	}
}  
Output:

Compile time error

*/

/*
P26:After type cast:

class OperatorExample
{  
	public static void main(String args[])
	{  
		short a=10;  
		short b=10;  
		a=(short)(a+b);//20 which is int now converted to short  
		System.out.println(a);  
	}
}  
Output:

20

*/
//-------------------------------------------------------------------------
/*
//Java Control Statements
P1:public class IfExample {  
public static void main(String[] args) {  
    int age=20;  
    if(age>18){  
        System.out.print("Age is greater than 18");  
    }  
}  
}  
Test it Now
Output:

Age is greater than 18

*/
/*
P2: public class IfElseExample {  
public static void main(String[] args) {  
    int number=13;  
    if(number%2==0){  
        System.out.println("even number");  
    }else{  
        System.out.println("odd number");  
    }  
}  
}  
Test it Now
Output:

odd number
*/

/*
//Java if-else-if ladder Statement
The if-else-if ladder statement executes one condition from multiple statements.

Syntax:

if(condition1)
{  
	//code to be executed if condition1 is true  
}
else if(condition2)
{  
	//code to be executed if condition2 is true  
}  
else if(condition3)
{  
	//code to be executed if condition3 is true  
}  
...  
else
{  
	//code to be executed if all the conditions are false  
}  
*/
/*
P3: Java if-else-if ladder Statement
public class IfElseIfExample 
{  
	public static void main(String[] args)
	{  
	    int marks=65;        
	    if(marks<50)
	    {  
		System.out.println("fail");  
	    }  
	    else if(marks>=50 && marks<60)
	    {  
		System.out.println("D grade");  
	    }  
	    else if(marks>=60 && marks<70)
	    {  
		System.out.println("C grade");  
	    }  
	    else if(marks>=70 && marks<80)
	    {  
		System.out.println("B grade");  
	    }  
	    else if(marks>=80 && marks<90)
	    {  
		System.out.println("A grade");  
	    }else if(marks>=90 && marks<100)
	    {  
		System.out.println("A+ grade");  
	    }
	    else
	    {  
		System.out.println("Invalid!");  
	    }  
	}  
}  
Output:

C grade
*/
/*
//Java Switch Statement
P4: public class SwitchExample
{  
	public static void main(String[] args) 
	 {  
	    //Declaring a variable for switch expression  
	    int number=20;  
	    //Switch expression  
	    switch(number){  
	    //Case statements  
	    case 10: System.out.println("10");  
	    break;  
	    case 20: System.out.println("20");  
	    break;  
	    case 30: System.out.println("30");  
	    break;  
	    //Default case statement  
	    default:System.out.println("Not in 10, 20 or 30");  
    	}  
    }  
}  
*/

/*
P5:

public class Switch
{
	public static void main(String args[])
	{
	    int age = 3;
	    switch(age)
	    {
	        case 1:
	                System.out.println("your age is: 1");
	                break;
	        case 2: 
	                System.out.println("your age is: 2");
	                break;
	        case 3:
	                System.out.println("your age is: 3");
	                break;
	        case 4:
	                System.out.println("your age is: 4");
	                break;
	        default: System.out.println("not in 1, 2, 3, 4");
	    }
	}
}

O/P:
  

*/

/*
P6: Finding Month Example:

//Java Program to demonstrate the example of Switch statement  
//where we are printing month name for the given number  
public class SwitchMonthExample 
{    
	public static void main(String[] args)
	{    
		    //Specifying month number  
		    int month=7;    
		    String monthString="";  
		    //Switch statement  
		    switch(month){    
		    //case statements within the switch block  
		    case 1: monthString="1 - January";  
		    break;    
		    case 2: monthString="2 - February";  
		    break;    
		    case 3: monthString="3 - March";  
		    break;    
		    case 4: monthString="4 - April";  
		    break;    
		    case 5: monthString="5 - May";  
		    break;    
		    case 6: monthString="6 - June";  
		    break;    
		    case 7: monthString="7 - July";  
		    break;    
		    case 8: monthString="8 - August";  
		    break;    
		    case 9: monthString="9 - September";  
		    break;    
		    case 10: monthString="10 - October";  
		    break;    
		    case 11: monthString="11 - November";  
		    break;    
		    case 12: monthString="12 - December";  
		    break;    
		    default:System.out.println("Invalid Month!");    
	    }    
    			//Printing month of the given number  
   			 System.out.println(monthString);  
	}    
}   
*/
/*
P7: //Java Switch Example where we are omitting the  
//break statement  
public class SwitchExample2 {  
public static void main(String[] args) {  
    int number=20;  
    //switch expression with int value  
    switch(number){  
    //switch cases without break statements  
    case 10: System.out.println("10");  
    case 20: System.out.println("20");  
    case 30: System.out.println("30");  
    default:System.out.println("Not in 10, 20 or 30");  
    }  
}  
}  
O/P:
----
20
30
Not in 10, 20 or 30

*/

/*
P8: //Java Program to demonstrate the use of Java Switch  
//statement with String  
public class SwitchStringExample {    
public static void main(String[] args) {    
    //Declaring String variable  
    String levelString="Expert";  
    int level=0;  
    //Using String in Switch expression  
    switch(levelString){    
    //Using String Literal in Switch case  
    case "Beginner": level=1;  
    break;    
    case "Intermediate": level=2;  
    break;    
    case "Expert": level=3;  
    break;    
    default: level=0;  
    break;  
    }    
    System.out.println("Your Level is: "+level);  
}    
}
O/P:
Your Level is: 3

*/
/*
P9:
//Java Program to demonstrate the use of Java Nested Switch  
public class NestedSwitchExample {    
    public static void main(String args[])  
      {  
      //C - CSE, E - ECE, M - Mechanical  
        char branch = 'C';                 
        int collegeYear = 4;  
        switch( collegeYear )  
        {  
            case 1:  
                System.out.println("English, Maths, Science");  
                break;  
            case 2:  
                switch( branch )   
                {  
                    case 'C':  
                        System.out.println("Operating System, Java, Data Structure");  
                        break;  
                    case 'E':  
                        System.out.println("Micro processors, Logic switching theory");  
                        break;  
                    case 'M':  
                        System.out.println("Drawing, Manufacturing Machines");  
                        break;  
                }  
                break;  
            case 3:  
                switch( branch )   
                {  
                    case 'C':  
                        System.out.println("Computer Organization, MultiMedia");  
                        break;  
                    case 'E':  
                        System.out.println("Fundamentals of Logic Design, Microelectronics");  
                        break;  
                    case 'M':  
                        System.out.println("Internal Combustion Engines, Mechanical Vibration");  
                        break;  
                }  
                break;  
            case 4:  
                switch( branch )   
                {  
                    case 'C':  
                        System.out.println("Data Communication and Networks, MultiMedia");  
                        break;  
                    case 'E':  
                        System.out.println("Embedded System, Image Processing");  
                        break;  
                    case 'M':  
                        System.out.println("Production Technology, Thermal Engineering");  
                        break;  
                }  
                break;  
        }  
    }  
}  
O/P:
Data Communication and Networks, MultiMedia

*/

/*
P10: 
//Java Program to demonstrate the use of Enum  
//in switch statement  
public class JavaSwitchEnumExample {      
       public enum Day {  Sun, Mon, Tue, Wed, Thu, Fri, Sat  }    
       public static void main(String args[])    
       {    
         Day[] DayNow = Day.values();    
           for (Day Now : DayNow)    
           {    
                switch (Now)    
                {    
                    case Sun:    
                        System.out.println("Sunday");    
                        break;    
                    case Mon:    
                        System.out.println("Monday");    
                        break;    
                    case Tue:    
                        System.out.println("Tuesday");    
                        break;         
                    case Wed:    
                        System.out.println("Wednesday");    
                        break;    
                    case Thu:    
                        System.out.println("Thursday");    
                        break;    
                    case Fri:    
                        System.out.println("Friday");    
                        break;    
                    case Sat:    
                        System.out.println("Saturday");    
                        break;    
                }    
            }    
        }    
} 
O/P:
Sunday
Monday
Twesday
Wednesday
Thursday
Friday
Saturday

*/
/*
P11:
//Java Program to demonstrate the use of Wrapper class  
//in switch statement  
public class WrapperInSwitchCaseExample {       
       public static void main(String args[])  
       {         
            Integer age = 18;        
            switch (age)  
            {  
                case (16):            
                    System.out.println("You are under 18.");  
                    break;  
                case (18):                
                    System.out.println("You are eligible for vote.");  
                    break;  
                case (65):                
                    System.out.println("You are senior citizen.");  
                    break;  
                default:  
                    System.out.println("Please give the valid age.");  
                    break;  
            }             
        }  
}  

O/P:
You are eligible for vote.
*/

/*
P11: Loops in Java: 1. for loop 2. while loop 3. do-while loop
public class ForExample {  
public static void main(String[] args) {  
    //Code of Java for loop  
    for(int i=1;i<=10;i++){  
        System.out.println(i);  
    }  
}  
}  


*/
