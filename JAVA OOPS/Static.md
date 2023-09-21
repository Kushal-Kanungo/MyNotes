The static can be:

1. Variable (also known as a class variable)
2. Method (also known as a class method)
3. Block
4. Nested class

#### There are two main restrictions for the static method. They are:

1. The static method can not use **non static data member** or call non-static method directly.
2. this and super cannot be used in static context.

## 3) Java static block

- Is used to initialize the static data member.
- It is executed before the main method at the time of classloading.

```java
class A2{  
  static{System.out.println("static block is invoked");}  
  public static void main(String args[]){  
   System.out.println("Hello main");  
  }  
}  
```