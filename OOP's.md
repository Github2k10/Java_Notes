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
