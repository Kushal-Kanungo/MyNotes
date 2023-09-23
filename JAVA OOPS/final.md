The **final keyword** in java is used to restrict the user. The java final keyword can be used in many context. Final can be:

1. variable
2. method
3. class

#### Final Variable
- **cannot change** the value of final variable(It will be constant).

#### Final Method
- any method as final, you cannot override it.

#### Final Class
- any class as final, you cannot extend it.

### IMP QUESTIONS

#### Q) is final methods inherited ?
> Yes, but we cannot override them.

#### Q) What is blank or uninitialized final variable?

> A final variable that is not initialized at the time of declaration is known as blank final variable.
>
> If you want to create a variable that is initialized at the time of creating object and once initialized may not be changed, it is useful. For example PAN CARD number of an employee.
> 
 It can be initialized only in constructor.

#### Q) Can we initialize blank final variable?
> Yes but only in constructor not after that

```java
class Bike10{  
  final int speedlimit;//blank final variable  
    
  Bike10(){  
	  speedlimit=70;  
	  System.out.println(speedlimit);  
  }  
  
  public static void main(String args[]){  
    new Bike10();  
 }  
}  
```

#### Q) static blank final variable

> A static final variable that is not initialized at the time of declaration is known as static blank final variable. It can be initialized only in static block.

```java
class A {  
	static final int data;//static blank final variable  
		static{ data=50;}  
		public static void main(String args[]){  
		System.out.println(A.data);  
	}  
}  
```

#### Q) What is final parameter?
> If you declare any parameter as final, you cannot change the value of it.

