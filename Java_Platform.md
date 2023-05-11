# Part-1: Java Platform

**1. Why is Java so Popular?**
> *Answer:* There are several reasons that make java a very popular programming language:
> 1. Platform Independence: Java is platform independent language means we can run java code on any platform such as Mac, linux, Windows, etc. that has a Java Virtual Machine(JVM). This makes java very attractive to most of the developers because they don't need to write code for any specific operatic system. It allows them to write once and run anywhere.
>
> 2. Object-Oriented Programming: Java is object-oriented programming language, which means that it allows a developer to create reusable code components(object) that can be easily modified and reused in different parts of the program. This makes Java code more modular, maintainable, and scalable.
>
> 3. High Performance: Java provides high performance with the use of "JIT" Just In Compiler, in which the compiler compiles the code on a demand basis, that is it compiles only that method which is being called. This saves the time and makes it more efficient, and even better performs on large-scale, complex applications.
>
> 4. Security: Java is best known for security. It has a strong security built into the language, which helps to protect against common security vulnerabilities such as buffer overflows and memory leaks.
>
> Apart from this, there are many more features in java that make java a popular language, like; Architecture-neutral language, portable, distributed, multi-threaded and interactive, dynamic, etc.

<br> <br>

**2. What is Platform Independence?**
> *Answer:* Platform independence is an ability of software or code that can run on any hardware and software platform without any modification. As the java is a platform independent language, we can execute java code on multiple platform like; windows, Mac, linux, Android, etc. Java code is compiled by the compiler and converted into bytecode. This bytecode is a platform independent code that can run on any platform that has Java Virtual Machine (JVM). That's way java also called WORA (Write Once and Run Anywhere).

<br> <br>

**3. What is ByteCode?**
> *Answer:*
> Bytecode is a binary format of a program or code
> that represents the intermediate form of the program written in the high-level language such as Java.
> When we compile our code, it is translated into bytecode,
> which is set of instructions that can be executed by the JVM in this case.
> The JVM acts as an interpreter
>, and it will translate that bytecode into machine language that can we executed by the host computer processer.
> <br>
> As the bytecode is platform independent that can be run on any operating system or any platform.
> The JVM provides a layer of abstraction between the bytecode and the underlying hardware,
> allowing Java programs to be executed on different platforms without any modifications.

<br> <br>

**4. Compare JDK vs JVM VS JRE.**
> *Answer:* 
> | JDK | JVM | JRE |
> |-----|-----|-----|
> | Java Development Kit | Java Virtual Machine | Java Runtime Environment |
> | It is a software development kit tot develop applications in java. In addition to JRE, JDK also contains number of development tools. | It is an abstract machine that is platform-dependent and has three notions as a specification, a document that describes requirement of JVM implementation, implementation, a computer program that meets JVM requirements, and instance, an implementation that executes Java byte code provides a runtime environment for executing java byte code. | It is the implementation of JVM and is defined as a software package that provides Java class, libraries, along with JVM, and other components to run applications written in Java programming. |
> | It is platform dependent | It is platform independent. | It is also platform dependent. |
> | It is responsible for prime development, so it contains tools for developing, debugging and monitoring java application. | It does not include software development tools. | It does not contain tools such as compiler or debugger etc. Rather it contains class libraries and another supporting filer that JVM requires to run the program. |
> | JDK = JRE + Development tools | JVM = Only Runtime environment for executing the Java byte code. | JRE = JVM + libraries to run the application | 

 <br> <br>

 **5. What is the role of class loader in java?**
 > *Answer:* In java, a class loader is a component of the JRE that loads Java classes into the JVM at runtime. The main role of the class lander is to locate the bytecode of a Java class file into memory so that it can be executed by the JVM. <Br>
 > Some other key role of class loader in Java: <br>
 > 1. Namespace Management: The class loader is also responsible for creating spear namespace for each class it loads, to ensure that each class has a unique identity.
 > 2. Security: The class loader also plays a key role in enforcing Java's security model by checking whether the loaded classes are trusted or not.
 > 3. Dynamic loading: Class loader allows dynamic loading of classes at runtime, which enables Java programs to load classes as needed, rather than loading all classes at startup.

 <br> <br>
