
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

**3. What is the need for finally block?**
> *Answer:* The finally block in exception handling serves an important purpose by allowing us to specify code that will be executed regardless of whether an exception occurred or not. The 'fianlly' block is executed regardless of whether an exception is thrown and caugth or progagtes up the call stack. 'finally' block is used for many purposes like reource cleanup, guaranteeing execution, consistency and maintainability, etc.

<br> <br>

**4. In what scenarios is code in finally not executed?**
> *Answer:* Although, in most of the scenarios the 'finally' block will execute. But here are few scenarios in which finally block will not execute: <br>
> - System exit: if the program terminated abruptly using 'System.exit()' before reaching the 'finally' block, the code within the finally block will not be executed. <br>
> - Infinite loop or deadlock: If the code within the 'try' or 'catch' blocks enters an infinite loop or encounters a deadlock situation. preventing the program from progressing, the 'finally' block may not be exceuted. <br>
> - Unhandled exceptions: If an unhandled exception occurs in the 'try' block, which propagates up the call stack and is not caught by any catch block, the 'finally' block may not be executed. 

<br> <br>

**5. Is try without a catch is allowed?**
> *Answer:* Yes, it is allowed to have a 'try' block without a corresponding 'catch' block in java. However, if we omit the 'catch' block, we must include a 'finally' block to handle the exception or perform necessary cleanup operations.

<br> <br>

**6. Can you explain the hierarchy of Exception Handling classes?**
> *Answer:* java.lang.Throwable class is the root of hierarchy of Exception Handling classes. It is the super class of all the exception and errors calsses. <br>
> Exception is the subclass of 'Throwable' that represents exceptional conditions that can be caugth and handled by the program. <b>
> 'java.lang.RuntimeException' is a subclass of 'Exception' that represents exceptions that can occure during runtime and are typically unchecked. They do not need the explicitly declared or caught. <br>
> 'java.lang.Erro' is another subclass of 'Throwable' that represents serious errors that are typically caused by external factores or conditions beyond the control of the program. <br>
> Here's the hierarchy of Exception classes: <br>
>
> Throwable
> - Exception
>   - IOException
>   - SQLException
>   - ClassNotFoundException
>   - RuntimeException
>     - ArithmeticException
>     - NullPointerException
>     - NumberForamtException
>     - IndexOutOfBoundException
> 
> - Error
>   - StackOverflowError
>   - VirtualMachineError
>   - OutOfMemeoryError

<br> <br>

**7. What is the difference between Error and Exception?**
> *Answer:* <br>
> | Error | Exception |
> | ----- | --------- |
> | Error cannot be recoverd. | Exception can be recovered by using the try-catch block. |
> | All errors in java are unchecked. | Exceptions are classified into two parts ie. checked and unchecked. |
> | It occurs at run time. | It occurs at compile time or run time. |
> | It belongs to java.lang.Error package. | it belongs to java.lang. Exception package. |
> | It will not be known to the compiler. | Only checked exceptions are known to the compiler. |
> | It is mostly caused by the environment in which the application is running. | It is mainly caused by the application itself. |
> | StackOverFlow, OutOfMemeoryError are the example of Error. | SQLException, NullPointerException are the example of Exception. | 

<br> <br>
