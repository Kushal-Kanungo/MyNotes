z
```java
//Java Program to demonstrate having the main method in   
//another class  
//Creating Student class.  
class Student{  
 int id;  
 String name;  
}  
//Creating another class TestStudent1 which contains the main method  
class TestStudent1{  
 public static void main(String args[]){  
  Student s1=new Student();  
  System.out.println(s1.id);  
  System.out.println(s1.name);  
 }  
}  
```

3 Ways to initialise object variables

1. Using reference variable name
```java
class Student{  
  int id;  
  String name;  
 }  
class TestStudent2{  
	public static void main(String args[]){  
	Student s1=new Student();  
	s1.id=101;  
	s1.name="Sonoo";  
		System.out.println(s1.id+" "+s1.name);//printing members with a white space  
  }  
 }
```

2. Using **Constructors**
3. Using methods like **setters** and other methods.

#### Different ways to create objects

- By **new** keyword
- By **newInstance()** method
- By **clone()** method
- By **deserialization**
- By **factory method** etc.

#### Anonymous Object

Calling method through an anonymous object
```java
new Calculation().fact(5);  
```
