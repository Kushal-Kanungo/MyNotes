A class which is declared with the **abstract keyword** is known as an abstract class in [Java](https://www.javatpoint.com/java-tutorial). It can have **abstract** and **non-abstract methods** (method with the body).

#### IMP Rules
- An abstract class must be declared with an abstract keyword.
- It can have abstract and non-abstract methods.
- It cannot be instantiated.
- It can have [[Constructor]]s and static methods also.
- It can have final methods which will force the subclass not to change the body of the method.

#### Abstract Methods in Java
A method which is declared as abstract and does not have implementation is known as an abstract method.

**Imp:** Abstract method cannot exist without **abstract class** or **interface** 

```java
abstract class Bike{  
	abstract void run();  
}  

class Honda4 extends Bike{  
	void run() { 
		System.out.println("running safely");
	}
	  
	public static void main(String args[]) {  
		Bike obj = new Honda4();  
		obj.run();  
	}  
}  
```

#### Abstract Class can have
- Data Members
- Abstract Method
- Method Body
- Constructor
- Main() method