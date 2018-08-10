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




