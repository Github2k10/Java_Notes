# Part-2: Wrapper Classes

**1. What are wrapper classes?**
> *Answer:* 
Java is a fully object-oriented programming language, but it includes primitive data types such as int, char, boolean, etc., which are not objects. To overcome this limitation and make these primitive types more versatile, Java introduced wrapper classes. These classes provide a way to use primitive data types as objects and offer additional functionalities through their methods. <br>
> By using wrapper classes, developers can convert a primitive data type to an object, perform operations on the object, and convert it back to the primitive type when necessary. For example, the Integer class provides methods to convert an int to a String, compare two int values, and perform mathematical operations such as addition, subtraction, etc.

<br> <br>

**2. Why do we need Wrapper Classes in Java?**
> *Answer:* Wrapper classes provide several advantages, such as:
> 1. Allows primitive data types to be used as objects: As wrapper classes provide object-oriented methods to manipulate primitive data types, it makes it easier to use them in object-oriented programming.
> 2. Provides useful methods: Wrapper classes provide methods to convert between primitive data types and strings, compare values, and perform other useful operations.
> 3. Enables compatibility with Java Collection Framework: As the collection framework works with objects, wrapper classes are needed to store primitive data types in collections such as ArrayList, HashSet, etc.
> 4. Autoboxing and unboxing: Java provides automatic conversion between primitive data types and their corresponding wrapper classes. This is called autoboxing and unboxing, which allows develops to use both primitive types and objects and objects interchangeably, making code more concise and easier to read.

<br> <br>

**3. What are the different ways of creating Wrapper Class Instances?**
> *Answer:* There are several ways to create instance of wrapper classes in java. Some of are:
> 1. Using Constructors: Wrapper class is itself a class, so it has their own constructor. With the help of this constructor, we can easily create an instance of wrapper class. Example: Integer myInt = new Integer(10);
> 2. Using valueOf() method: All wrapper classes (except Character) have a static method "valueOf()" method that can be used to create an object from a string or a primitive data type. Example: Integer myInt = Integer.valueOf(10)/valueOf("10");
> 3. Using autoboxing: Java provides automatic conversion between primitive data types and their corresponding wrapper classes. This is called autoboxing, and it allows us to create a wrapper object implicitly. Example: Integer mayInt = 10;
> 4. Parsing Strings: Wrapper classes (except Character) also provide a static "paseXXX()" method that can be used to create objects from a string. Example: Integer myInt = Integer.parseInt("10");

<br> <br>

**4. What are differences in the two ways of creating wrapper classes?**
> *Answer:* The two common ways of creating instances of wrapper classes in java are using constructors and using the valueOf() method. Here are the differences between these two of them:
> 1. Constructor vs Static method: The primary difference is that constructor is instance member function, while "valueOf()" is static function.
> 2. Performance: The valueOf() method is generally more efficient as compared to constructor.
> 3. Handling Null Values: When passing null to constructor, it will throw "NullPointerException" at runtime. However, when passing null to valueOf() method, it will throw "NullPointerException" at compile time.
> 4. Widening Conversion: Constructors of wrapper classes accept a wide range of input types, including widening conversions, while the valueOf() method only accepts the exact same type.

<br> <br>

**5. What is Auto Boxing?**
> *Answer:* Auto boxing is a feature that allows automatic conversion between primitive data types and their corresponding wrapper classes. With auto boxing, we can use primitive data types where objects are required, and vice-versa, without having to manually convert them. <br>
> Example: <br>
> int i = 10; <br>
> Integer myInt = i;

<br> <br>

**6. What are the advantages of Auto Boxing?**
> *Answer:* Auto boxing eliminates the need for manual conversion between primitive data types and their corresponding wrapper classes, which can simplify code and make is more readable. <br>
> There are many other advantages that provide auto boxing like, improve interoperability, enable use of collections, reduce errors, and support generics.

<br> <br>

**7. What is Casting?**
> *Answer:* In java, type casting or casting is a method or process that converts a data type into another data type in both ways manually and automatically. The automatic conversion is done by the compiler and manual conversion performed by the programmer. It involves specifying the target data type in parentheses before the value being cast <br>
> There are two types of casting: Narrowing Type casting or explicit conversion and Widening type casting or implicit conversion.

<br> <br>

**8. What is Implicit Casting?**
> *Answer:* Converting a lower data types into higher one is called implicit casting. It is also known as widening type casting or down casting. It is done automatically. It is safe because there is no chance to lose data. <br>
> It takes place when: <br>
> Both data types must be compatible with each other. <br>
> The target type must be larger than the source type. <br> <br>
> byte -> short -> char -> long -> float -> double <br>
> Example: the conversion between numeric data type to char or boolean is not done automatically. Also, the char and boolean data types are not compatible with each other.

<br> <br>

**9. What is Explicit Casting?**
> *Answer:* The converting a higher data type into a lower one is called explicit casting. It is also known as narrowing conversion or up casting. It is done manually by the programmer. If we do not perform the casting the compiler will throw an error. <br>
> double -> float -> long -> int -> char -> short -> byte <br>
> Example: long l = (long)d;
