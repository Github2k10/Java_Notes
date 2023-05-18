
Part-8: Exception Handling

**1. Why is Exception Handling important?**
> *Answer:* Exception Handling in Java is a mechanism to handle runtime erros or exception that can occure in the program due to any abnormal condition such as ClassNotFoundException, IOException, SQLException, etc. <br>
> It is important to handle this type of exception to handle to maintain the noraml flow of the application. <br>
> - Handling Exception provides a mechanism to handle and recover from erros and exceptional situations in a structured and controlled manner. <br>
> - We can make our code more robust and reliable. <br>
> - Exceptions handling help in the debugging and troubleshooting process. When an exception occurs, it provides valuable information about the error. <br>
> - Proper exceptions handling promotes code maintainability and readibility. <br>
> - Exception handling allows us to gracefully recover from errors and provides a better user experience.

<br> <br>

**2. What design pattern is used to implement Exception handling Features in most languages?**
> *Answer:* 'Chain of Responsibility' design pattern is used to implement Exception handling Features in most languages. This provides a structured apporach to handling exceptions and is typcially implemented using a combination of try-catch blocks. <br>
> Here's how the Exception Handling design pattern works:
> - Try block: The code that might throw an exception is enclosed withing a try block. If an exception occurs within the try block, the normal flow of execution is interrupted, and the corresponding catch block is searched for to handle the exception. <br>
> - Catch block: A catch block follow the try block and specifies the type of exception it can handle. If an exception of that type is thrown within the try block or any of its nested blocks, the catch block is executed. Multiple catch blocks can be chained together to handle different types of exceptions. <br>
> - Finally block(optional): Optionally, a finaly block can be used after the catch block. The code within the finally block is executed regardless of whether an exception occurred or not. It is typically used to perform cleanup operations or release resoures.

<br> <br>
