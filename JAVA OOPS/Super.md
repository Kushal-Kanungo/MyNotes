The **super** keyword in Java is a reference variable which is used to refer immediate parent class object.

Whenever you create the instance of subclass, an instance of parent class is created implicitly which is referred by super reference variable.

1. **super** can be used to refer immediate parent class instance variable.
2. **super** can be used to invoke immediate parent class method.
3. **super()** can be used to invoke immediate parent class constructor.

#### Refer parent class instance variable
```java
class Animal{  
	String color="white";  
}  

class Dog extends Animal{  
	String color="black";  
	void printColor(){  
		System.out.println(color);//prints color of Dog class  
		System.out.println(super.color);//prints color of Animal class  
	}  
}  

class TestSuper1{  
	public static void main(String args[]){  
		Dog d=new Dog();  
		d.printColor();  
	}
}  
```

#### Invoke parent class methods
```java
class Animal{  
	void eat(){System.out.println("eating...");}  
}  

class Dog extends Animal{  
	void eat(){System.out.println("eating bread...");}  
	void bark(){System.out.println("barking...");}  
	void work(){  
		super.eat();  
		bark();  
	}  
}  
class TestSuper2{  
	public static void main(String args[]){  
		Dog d=new Dog();  
		d.work();  
	}
}  
```

#### **Invoke Parent class constructor**

- By default, parent class **constructor** invoked automatically in java if we do not define **super()** explicitly.
- **super()** is useful when there are **multiple constructor** in the parent class and we want to invoke a particular constructor according to arguments.

```java
class Person{  
	int id;  
	String name;

	// Parameterized Constructor
	Person(int id,String name){  
		this.id=id;  
		this.name=name;  
	}  
}  

class Emp extends Person{  
	float salary; 
	 
	Emp(int id,String name,float salary){  
		super(id,name);//reusing parent constructor  
		this.salary=salary;  
	}
	  
	void display() { 
		System.out.println(id+" "+name+" "+salary);
	}  
}  

class TestSuper5{  
	public static void main(String[] args) {  
		Emp e1=new Emp(1,"ankit",45000f);  
		e1.display();  
	}
}  
```