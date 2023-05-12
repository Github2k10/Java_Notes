# Part-3: Strings

**1. Are all String’s immutable?**
> *Answer:* Yes, In java all strings are immutable (expected StringBuilder and StringBuffer). This means that once a string is created, its contents cannot be modified. Any operation that appears to modify a string actually creates a new string with the modified content, leaving the original string unchanged.

<br> <br>

**2. Where are string values stored in memory?**
> *Answer:* In java, string values are stored in a special memory area called string pool or string constant pool. <br>
> When a string is created using a string literal, such as "Java", java first checks if the string is already present in the string pool. If the string is not present, java creates a new string a new string object and adds it to the pool. If the string is already present in the pool, java simply returns a reference to the existing string object in the pool.

<br> <br>
**3. Why should you be careful about String Concatenation(+) operator in Loops?**
> *Answer:* In java, '+' operator is used to create a new string object by concatenating the strings. When we are using concatenation in a loop, it will create a new string each time that lead to a significant number of string objects being created, which can have a negative impact on performance and memory usage.

<br> <br>
**4. How do you solve above problem?**
> *Answer:* To avoid this problem, it is recommended to use 'StringBuilder' or 'StringBuffer' instead of the '+' operator for string concatenation in loops. These classes provide more efficient ways to build strings, by creating a single mutable buffer for the string and appending to it in each iteration of the loop. 

<br> <br>
**5. What are differences between String and StringBuffer?**
> *Answer:* <br>
> | String | StringBuffer |
> | ------ | ------------ |
> | The string class is immutable. | The StringBuffer class is mutable. |
> | It is slow and consumes more memory when we concatenate strings. | It is fast and consumes less memory when we concatenate strings. |
> | String class overrides the equals method of Object class to perform comparison. | StringBuffer class doesn't override the equal method for comparing two strings. |
> | String class uses string constant pool. | StringBuffer uses heap memory. |

<br> <br>
**6. What are differences between StringBuilder and StringBuffer?**
> *Answer:* <br>
> | StringBuilder | StringBuffer |
> | ------------- | ------------ |
> | StringBuilder is non-synchronized. | StringBuffer is synchronized. |
> | StringBuilder is not thread safe. | StringBuffer is thread safe, means two threads can't call the methods of StringBuffer simultaneously. |
> | StringBuilder is more efficient than StringBuffer. | StringBuffer is less efficient than StringBuilder. |
> | StringBuilder was introduced in java 1.5. | StringBuffer was introduced in java 1.0. |

<br> <br>
