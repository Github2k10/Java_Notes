# Part-4: OOP's

**1. What is a Class?**
> *Answer:* In java, a class is a blueprint or template that defines the characteristics and behavior of an object. It is a fundamental concept in object-oriented programming and is used to create objects, which is instance of class. <br>
> A class consist of data field(variables) and methods(functions) that define the properties and behavior of the objects created from the class. The data fields represent the object's state or properties, and the methods represent the object's behavior or actions. <br>
> Syntax:
> class class_Name{ //Variables and methods }
> 
<br> 
<br>

**2. What is state of object?**
> *Answer:* The state of an object in Java refers to the current values of its attributes or properties (represented by instance variables), which can change over time as the object's methods are invoked and its state is modified. <br>

<br> <br>

**3. What is behavior of an Object?**
> *Answer:* The behavior of an object in java refers to the actions or operations that the object can perform. These actions or operations are defined by the methods of the object class, and can be invoked by methods on the object. <br>
> In simpler terms, the behavior of an object refers to what the object can do or how it can interact with objects or the system as a whole.

<br> <br>

**4. What is the super class of every class in Java?**
> *Answer:* Object class is super class of every class.

<br> <br>

**5. Explain about toString method ?**
> *Answer:* In java, toString() method is defined in the object class, and it is inherited by all other classes. The purpose of the toString() method is to provide a string representation of the object. <br>
> The default implementation of the toString() method in the Object class returns a string that consists of the name of the object's class, followed by an '@' sign and the hexadecimal representation of the object's hash code.

<br> <br>

**6. What is the use of equals method in Java ?**
> *Answer:* In Java, the equals() method is defined in the Object class, and it is inherited by all other classes. The purpose of the equals() method is to determine whether two objects are equal. <br>
> The default implementation of the equals() method in the Object class simply compares two objects are reference equality, which means that is returns true only if the two object references point to the same object in memory.

<br> <br>

**7. What are the important things to consider when implementing equals method?**
> *Answer:* While implementing the equals() method in java class, there are several important things to consider:
> 1. The equals() method should always return the same result when called with the same object. <br>
> 2. The equals() method should always return true when called with the same object. <br>
> 3. The equals() method should always return false if it is called with a 'null' parameter. <br 
> 4. The equals() method should always return false if it is called with an object of a different class. <br>
> 5. The equals() method should always return true if it is called with an object having the same reference or pointing the same object. <br>
> 6. The equals() method should always compare the state of objects to determine equality. In other words, it should compare all the fields of the object that contribute to its identity. 

<br> <br>

**8. What is the hashCode method used for in Java?**
> *Answer:* In Java, the hashCode() method is used to generate a hash code (a unique identifier) for an object. The hash code is an integer value that is used to identify in hash-based data structures such as hash tables, hash maps, and hash sets. <br>
> It is necessary ot override the hashCode() methode in a class to provide a more meaningful hash code based on the state of the object. If two objects are equals, according to their equals() method, they should be also have the same hash code. 

<br> <br>

**9. Explain inheritance with Examples?**
> *Answer:* Inheritance in java is a mechanism in which one class acquires all the properties and behaviors of a parent class. The idea behind inheritance in java is that we can create new classes that are built upon existing classes. When we inherit from an existing class, we can reuse methods and fields of the parent class. <br>
> Inheritance represents the IS-A relationship which is also known as a parent-child relationship. <br>
> extends keyword is used to inherit an existing class. <br>
> Syntax: class SubClass_Name extends SuperClass_Name{} <br> <br>
> Example: <br>
> class vehicle { <br>
>   void print(String str){ System.out.println(str); } <br>
> } <br> <br>
> class Car extends vehicle{ <br>
>   void start(){ print("car started")}; <br>
>   void stop(){ print("car stopped");} <br>
> }

<br> <br>

**10. What is Method Overloading?**
> *Answer:* Method overloading is a feature in java that allows a class to have multiple methods with the same name, but different signature. When a method is overloaded, it has the same name as another method have in the same class, but the number of parameters or type of parameters of the two or more methods are different. This allows the programmer to reuse the same method name in different contexts, improving the readability and maintainability of the code. 

<br> <br>

**11. What is Method Overriding?**
> *Answer:* Method overriding is a feature in java that allows a subclass to override or re-define a method with their own implementation that is already defined in the superclass. When a method is overridden, it has the same name, return type, and parameter list as the method in the superclass have, but with a different implementation.

<br> <br>

**12. Can super class reference variable can hold an object of subclass?**
> *Answer:* Yes, a superclass reference variable can hold an object of a subclass. This is known as upcasting, and it allows for polymorphic behavior in Java.

<br> <br>

**13. Is Multiple Inheritance allowed in Java?**
> *Answer:* Java does not support multiple inheritance of classes, means a class cannot inherit from more than one class or one class cannot not have more than one parent class at the same time. This can lead ot ambiguities in the inheritance hierarchy and make the code harder to maintain.

<br> <br>

**14 What is an Interface ?**
> *Answer:* In Java, an interface is a collection of abstract methods (method with body) and constants (field that cannot be changed) that can be implemented by a class that implements the interface. <br>
> Syntax: <br>
> public interface Interface_Name{ <br>
> void method1(); <br>
> void method2(): <br>
> }

<br> <br>

**15. How do you define an Interface ?**
> *Answer:* In java, an interface is defined by using 'interface' keyword, followed by the name of interface and a block containing at least one abstract method. <br>
> Example: <br>
> public interface MyInterface{ <br>
> void print(); <br>
> int const = 45; <br>
> }

<br> <br>

**16. How do you implement an interface?**
> *Answer:* To implement an interface in java, we need to create a class using 'implements' keyword followed by the interface name after the class name. Also provide an implementation for all the abstract methods of the interface. <br>
> Example: <br>
> interface MyInterface{ <br>
> public void show(); <br>
> } <br>
> public class MyClass implements MyInterface{ <br>
> public void show(){ <br>
> System.out.println("Inside show method of class"); <br>
> }

<br> <br>

**17 Can you explain a few tricky things about interfaces?**
> *Answer:* Here are a few tricky things about the interfaces in java: <br>
> 1. In Java 8 and later versions, interface can contain default methods that provide a default implementation for a method. Default method is defined by using 'default' keyword. <br>
> 2. In Java 8 and later versions, interface can contain static methods that can be called on the interface itself, not just on instance of classes that implement the interface. <br>
> 3. Interface in java support multiple inheritance.
> 4. All the methods are public, and all variables are public, static and final in interface. <br>
> 5. Interface cannot contain instance variables. They can only contain public static final constants, which are also called static fields.
> 6. Functional interface is an interface that has only one abstract method.

<br> <br>

**18. Can you extend an interface?**
> *Answer:* An interface can extend other interfaces, just as a class or subclass extend another class.

<br> <br>

**19. Can a class implements multiple interfaces?**
> *Answer:* Yes, we can implement multiple interfaces in java by separating the interface names with commas after the 'implements' keyword in the class declaration. <br.
> Syntax: public class implements Interface1, Interface2, Interface3 { // body of class }

<br> <br>

**20. What is an Abstract Class?**
> *Answer:* A class is declared with the abstract keyword is known as abstract class in java. It can have abstract and non-abstract methods (method with the body). <br.
> It's a way to define a common interface for a group of related classes, without providing a complete implementation. 

<br> <br>

**21. When do you use an Abstract Class?**
> *Answer:* Here are some use-cases of abstract classes: <br>
> 1. We can use an abstract class to define a set of methods that must be implemented by any subclass that inherits from it. <br>
> 2. We can use an abstract class to provide default implementations for some methods, while requiring that other methods be implemented by subclasses. <br>
> 3. We can use abstract class to define an interface that other classes can implement. 

<br> <br>

**22. How do you define an Abstract Method?**
> *Answer:* We can define an abstract method in an abstract class by using 'abstract' keyword in the method declaration, and omitting the method body. <br>
> Example: <br>
> public abstract class Shape{ <br>
> public abstract double area(); <br>
> public abstract double perimeter(); <br> }

<br> <br>

**23. Compare Abstract Class vs Interfaces?**
> *Answer:* <br>
> | Abstract Class | Interface |
> | -------------- | --------- |
> | It can have abstract and non-abstract methods. | It can only have abstract method. |
> | It doesn't support multiple inheritance. | It supports multiple inheritance. |
> | It can have final, non-final, static and non-static variables. | It has only static and final variables. |
> | It can provide the implementation of interface. | It can't provide the implementation of abstract class. |
> | abstract keyword is used to declare abstract class. | interface keyword is used ot declare interface. |
> | It can extends another Java class and implement multiple Java interface. | It can extend another java interface only. |
> | It can be extended using keyword 'extends'. | It can be implemented using keyword 'implements'. |
> | It can have class members like private, protected, etc. | Members of a java interface are public by default. |

<br> <br>

**24. What is a Constructor?**
> *Answer:* A constructor is a special method that is used to initialize objects. When an object is created using the 'new' keyword, a constructor is called to initialize the object's state. The constructor has the same name as the class and no return type. <br>
> Example: <br>
> public class Car{ <br>
> private String name; <br>
> public Car(String name){ this.name = name } // Constructor <br>
> }

**25. What is a Default Constructor?**
> *Answer:* A default constructor is a constructor that is automatically generated by the Java compiler if no other constructors are defined for a class. It is a constructor with no parameters, no explicit implementation, and an empty body. <br>
> Example: <br>
> public class Car{ <br>
> public Car(){} // default constructor <br>
> }

**26. How do you call a Super Class Constructor from a Constructor?**
> *Answer:* We can call a super constructor from a constructor of a subclass using the 'super()' keyword. The 'super()' keyword is used to call the constructor of the immediate superclass. It must be the first statement in the constructor body. <br>
> Example: <br>
> public class Vehicle{ <br>
> public Vehicle(){ System.out.println("Super class constructor"); } <br>
> } <br>
> 
> class Car extends Vehicle{ <br>
> public Car(){ <br>
> super(); // calling super constructor <br>
> System.out.println("constructor of subclass"); } <br>
> }

**27. What is the use of this()?**
> *Answer:* 'this()' is a special keyword that can be used inside a constructor to call another constructor of the same class. It is typically used to avoid duplicating code in multiple constructors. <br>
> It can also be useful for enforcing consistency across constructors in a class. <br>
> Example: <br>
> public class MyClass{ <br>
> public int value; <br> <br>
> public MyClass() { this(0); // call the constructor with a default value of 0 } <br>
> public MyClass(int value) { this.value = value; } <br> 
> }

<br> <br>

**28. Can a constructor be called directly from a method?**
> *Answer:* Yes, we can call constructor directly from a method to create an object of the respective class. <br>

<br> <br>

**29. Is a super class constructor called even when there is no explicit call from a subclass constructor?**
> *Answer:* Yes, a superclass constructor is always called, even if there is no explicit call from a subclass constructor. <br>
> When a subclass constructor is called, it implicitly calls the default constructor of its superclass. If the superclass has no default constructor, then the subclass constructor must explicitly call on of the superclass constructor's using the super() keyword. <br.

<br> <br>

**30. Difference between compile time and run time polymorphism?**
> *Answer:* <br>
> | compile time polymorphism | runtime polymorphism |
> | ------------------------- | -------------------- |
> | In this, the call is resolved by the compiler. | In this, the call is not resolve by the compiler. |
> | It is also known as static or early binding. | It is also known as dynamic or late binding. |
> | This is archived by method overloading. | This is archived by method overriding. |
> | It provides fast execution because the method that needs to be executed is known early at the compile time. | It provides slow execution as compare to early binding because the method that needs to be executed is known at the runtime. |
> | It is less flexible as all things execute at compile time. | It is more flexible as all things execute at run time. |
> | Inheritance is not involved. | Inheritance is involved. |
