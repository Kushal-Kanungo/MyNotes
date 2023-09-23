
> If a class has multiple methods having same name but different in parameters, it is known as **Method Overloading**.

#### There are two ways to overload the method in java

1. By changing number of arguments
```java
class Adder{  
	static int add(int a,int b) {
		return a+b;
	}  
	static int add(int a,int b,int c) {
		return a+b+c;
	}  
}  
	
class TestOverloading1 {  
	public static void main(String[] args) {  
		System.out.println(Adder.add(11,11));  
		System.out.println(Adder.add(11,11,11));  
	}
}  
```

2. By changing the data type of arguments
```java
class Adder{  
	
	static int add(int a, int b) {
		return a+b;
	}  
	
	static double add(double a, double b) {
		return a+b;
	}  
}  

class TestOverloading2{  
	
	public static void main(String[] args) {  
		System.out.println(Adder.add(11,11));  
		System.out.println(Adder.add(12.3,12.6));  
	}
}  
```

#### Can we overload java main() method?

Yes, by method overloading. You can have any number of main methods in a class by method overloading. But [JVM](https://www.javatpoint.com/jvm-java-virtual-machine) calls **main()** method which receives string array `String[] args` as arguments only. Let's see the simple example:

```java
class TestOverloading4 {  
	public static void main(String[] args) {
		System.out.println("main with String[]");
	}  
	public static void main(String args) {
		System.out.println("main with String");
	}  
	public static void main() { 
		System.out.println("main without args");
	}  
}  

// System.out.println("main with String[]");
```

#### Method overloading and type promotion
> One type is promoted to another implicitly if no matching datatype is found. Let's understand the concept by the figure given below:

```java
class OverloadingCalculation1{  
	void sum(int a,long b) {
		System.out.println(a+b);
	}
	  
	void sum(int a,int b,int c) {
		System.out.println(a+b+c);
	}  
  
	public static void main(String args[]) {  
		OverloadingCalculation1 obj=new OverloadingCalculation1();  
		obj.sum(20,20);//now second int literal will be promoted to long  
		obj.sum(20,20,20);  
		
	}  
}  
```