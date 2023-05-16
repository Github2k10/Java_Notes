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
