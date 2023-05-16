# Part-6: Modifiers

**1. What is default class modifier?**
> *Answer:* If a class doesn't have any access modifier like; 'public', 'private' or 'protected', then it is considered to have a default access modifier. This means that the class is only visible within the same package, and cannot be accessed from outside of the package. <br>
> Example: <br>
> package mypackage; <br> <br>
> class MyClass{ //body of class }

<br> <br>

**2. What is private access modifier?**
> *Answer:* When a member of a class declared with a private access modifier, it means that it can only be accessed from within same class, and not from any other class, even if they are in the same package. 'private' access modifer is used to restrict the access of class members, such as instance variable and methods, from the outside of the class. <br>
> Example: class A{ <br>
> private int k = 10;
> } <br> <br>
> class B{ <br>
> A a = new A(); <br>
> a.k = 20; // it will throw exception; <br>
> }

<br> <br>

**3. What is default or package access modifier?**
> *Answer:* When we declare a class, method, or instance variable without any access modifier, then it is considered to have a default access modifier. This means that the class, method, or instance variable can only visible or access within the same package, and cannot be accessed from outside of the package.
<br> <br>

**4. What is protected access modifier?**
> *Answer:* When we declare any method or instance variable with protected access modifier, this means that the method or instance variable can only accessible within the same package as the declaring class and within any subclasses in different package.

<br> <br>

**5. What is public access modifier?**
> *Answer:* The 'public' access modifier is used to specify that a class member(field, method, or nested class) is accessible from anywhere in the program. A public member can be accesseed by any other class in the same package or in any other package, and can be used as part of the public interface of a class or library. 

<br> <br>

**6. What access types of variables can be accessed from a Class in Same Package?**
> *Answer:* A class in the same package can access all variables with the 'default', 'protected', and 'public' access modifiers declared in another class within the same package.

<br> <br>

**7. What access types of variables can be accessed from a Class in Different Package?**
> *Answer:* A class in the different package can access all variables with the 'default', 'protected', and 'public' access modifiers declared in another class within the same package.

<br> <br>

**8. What access types of variables can be accessed from a Sub Class in Same Package?**
> *Answer:* A sub class in same package can access all variables with the 'default', 'protected', and 'public' access modifiers declared in another class within the same package.

<br> <br>

**9. What access types of variables can be accessed from a Sub Class in Different Package?**
> *Answer:* A sub class in the different package can access all variables with the 'protected' and 'public' access modifiers declared in another class within the same package.

<br> <br>

**10. What is the use of a final modifier on a class?**
> *Answer:* The 'final' modifier on a class means that the class cannot be extended or modified by any other class. This is used for security, efficiency, and design of the class.

<br> <br>

**11. What is the use of a final modifier on a method?**
> *Answer:* The 'final' modifier on a method means that the method cannot be overload or overridden by any subclass. 

<br> <br>

**12. What is a Final Variable?**
> *Answer:* A 'final' variable is a variable whose value cannot be changed once it has been initialized. 

<br> <br>

**13. What is a Final Argument?**
> *Answer:* A 'final' argument is a method parameter that is marked with the 'final' keyword. Once a method parameter is marked as 'final', its value cannot be changed withing the method.

<br> <br>
