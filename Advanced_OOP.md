# Part-5: Advanced OOP's

**1. What is Polymorphism?**
> *Answer:* Polymorphism is a fundamental concept in object-oriented programming (OOP) that allows objects of different classes to be treated as if they were of the same class. It is the ability of objects to take on different forms or behaviors depending on the context in which they are used. It is a powerful concept that allows for code readability and flexibility in OOP. <br>
> Example: if we have a superclass 'Animal' and two subclasses 'Dog' and 'Cat', then we can treat objects of both classes as 'Animal' object. 

<br> <br>

**2. What is the use of instanceof Operator in Java?**
> *Answer:* The 'instanceof' operator is used to check if an object is an instance of a particular class or interface. The operator returns a boolean value; 'true' if the object is an instance of the specified class or interface, and 'false' otherwise. <br>
> Example: myObject instanceof MyClass ? true : false ;

<br> <br>

**3. What is Coupling?**
> *Answer:* Coupling refers to degree of interdependence between classes or components within a software system. It is a measure of how closely connected two or more classes are, and how much they rely on each other of function. <br>
> In other words, we can say that it is used to check who much component B dependent on component A. If we make any change in component A, how it's reflected on component B.

<br> <br>

**4. What is Cohesion?**
> *Answer:* Cohesion refers to the degree to which the elements within a single module or component of a software system work together to achieve a specific purpose. It is a measure of how strongly related the functions and responsibilities of a module are to each other. <br>
> In other words, the more closely related stuff is grouped in a class, the higher will be the cohesiveness.

<br> <br>

**5. What is Encapsulation?**
> *Answer:* Encapsulation is a fundamental concept in object-oriented programming that refers to the practice of hiding the internal details of an object from the outside world and exposing only necessary interfaces or methods for interacting with it. It allows for better organization and abstraction of code, and provides a mechanism for data hiding and access control. <br>
> In Java, encapsulation is achieved through the use of access modifiers such as private, protected, and public. Private members or methods are only accessible within the same class, while protected members or methods are accessible within the same package and to subclass. Public members or methods are accessible to all classes and package. 

<br> <br>

**6. What is an Inner Class?**
> *Answer:* In Java, an inner class is a class that is defined within another class. It is also sometimes referred to as a nested class because it is nested inside another class. Inner class have access to the members of the outer class, including its private members, and can be used to encapsulate related functionality within a single class. <b>
> There are four types of inner classes in java: <br>
> 1. Member inner class: This is the most common type of inner class, and is defined at the member level of the outer class. It has access to the instance variables and methods of the outer class, and can be instantiated only within an instance of the outer class. <br>
> 2. Static inner class: This is an inner class that is marked as static. It does not have access to the instance of variables or methods of the outer class, but can be instantiated independently of any instances of the outer class. <br>
> 3. Local inner class: This in an inner class that is defined within a method or block of code. It has access to the local variables of the enclosing methods or block, and can only be used within that method or block. <br>
> 4. Anonymous inner class: This is a type of local inner class that does not have a name and is defined inline. It is typically used to define a class that implements an interface or extends a class without creating a separate subclass. <br>

<br> <br>

**7. What is a Static Inner Class?**
> *Answer:* Static inner class is an inner class that is marked as static. It does not have access to the instance of variables or methods of the outer class, but can be instantiated independently of any instances of the outer class. <br>
> Example: <br>
> public class OuterClass{ <br>
> private static int n = 20; <br> <br>
> public static class InnerClass{ <br>
> private int k; <br> <br>
> public InnerClass(int data){ <br>
> k = data; <br>
> } <br> <br>
> public int getN(){ return k;} <br>
> public int getK(){ return n;} <br>
> } <br>
>}

<br> <br>

**8. Can you create an inner class inside a method?**
> *Answer:* Yes, in java it is possible to define an inner class inside a method. This type of inner class is called a local inner class, and it is defined within the body of a method. <br>
> Example: <br>
> public class OuterClass{ <br>
> private int k = 10; <br> <br>
> public void example(){ <br>
> final int data = 20; <br> <br>
> class LocalInnerClass{ <br>
> public void printData(){ <br>
> System.out.println("Outer data: " + k); <br>
> System.out.println("inner data: " + data); <br>
> } <br>
> } <br> <br>
> LocalInnerClass innerClass = new LocalInnerClass(); <br>
> inner.printData(); <br>
> } <br>
> }

<br> <br>

**9. What is an Anonymous Class?**
> *Answer:* In Java, an anonymous clas is a local class that is declared and instantiated in a single expression, without assigning it to a variable or giving it a name. Anonymous classes are typically used to define a subclass of a class or implement an interface, without creating a separate class definition. <br>
> Example: <br>
> Thread thread = new Thread(new Runnable(){ <br>
> public void run(){ <br>
> System.out.println("Thread is running"); <br>
> } <br>
> });
