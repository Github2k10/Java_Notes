# Part-3: Strings

**1. Are all String’s immutable?**
> *Answer:* Yes, In java all strings are immutable (expected StringBuilder and StringBuffer). This means that once a string is created, its contents cannot be modified. Any operation that appears to modify a string actually creates a new string with the modified content, leaving the original string unchanged.

<br> <br>

**2. Where are string values stored in memory?**
> *Answer:* In java, string values are stored in a special memory area called string pool or string constant pool. <br>
> When a string is created using a string literal, such as "Java", java first checks if the string is already present in the string pool. If the string is not present, java creates a new string a new string object and adds it to the pool. If the string is already present in the pool, java simply returns a reference to the existing string object in the pool.

<br> <br>
