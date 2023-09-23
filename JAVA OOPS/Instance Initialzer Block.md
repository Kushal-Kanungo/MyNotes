> Instance Initializer block is used to initialize the instance data member. It run each time when object of the class is created.

#### Why use instance initializer block?
Suppose I have to perform some operations while assigning value to instance data member e.g. a for loop to fill a complex array or error handling etc.

```java
class Bike7{  
    int speed;  
      
    Bike7() { 
	    System.out.println("speed is "+speed);
	}  
   
    { speed=100; }  
       
    public static void main(String args[]){  
	    Bike7 b1=new Bike7();  
	    Bike7 b2=new Bike7();  
    }      
}  
```

#### Which called first between **constructor** and **instance initializer block** ?
ANS: **instance initializer block** invoked before **constructor** and after parent class constructor.

