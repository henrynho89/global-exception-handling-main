# global-exception-handling-main
In this video you will learn end to end implementation of Global Exception Handling in Spring boot with example. These is very important spring boot interview questions

github URL : https://github.com/codedecode25/globa...

Global Exception Handling Spring Boot | Spring boot exception handling controller advice | Live Demo

Q) Need of  Global Exception handling. Why to do Spring Boot Exception Handling? Global exception handling in spring boot needs?

In Real World projects, Its very important to handle errors correctly and simultaneously provide meaningful error messages to the clients too. Hence we need Exception handling in Spring boot , Spring Boot Exception Handling or Global exception handling in spring boot.
Today we will see how to properly handle errors specifically in spring boot.
Prerequisite : Spring boot, Creation of Rest APIs. Both of them we have covered in earlier videos. 

Q) How can we make Error response clear in spring boot exception handling

We are lucky enough that Spring already comes with the built in support for error handling. 
It’s our job to understand and implement it. And today we are going to do that to do exception handling in Spring Boot Application

Q) Annotation used for Spring Boot Error Handling 

For Exception handling in spring boot in global exception handling , we need following annotations - 

@RestController : is the base annotation for classes that handle REST operations.

@ControllerAdvice : The @ControllerAdvice annotation handles exceptions globally – it allows you to use the same ExceptionHandler for multiple controllers. This way, we can define how to treat an exception in just one place because this handler will be called whenever the exception is thrown from classes that are covered by ControllerAdvice.
as the name suggests, is “Advice” for multiple controllers.
allows our class to be a global interceptor of exceptions thrown by methods annotated by @RequestMapping.


@ExceptionHandler  : Spring annotation that provides a mechanism to treat exceptions that are thrown during execution of handlers (Controller operations). This annotation, if used on methods of controller classes, will serve as the entry point for handling exceptions thrown within this controller only. 

Altogether, the most common way is to use @ExceptionHandler on methods of @ControllerAdvice classes so that the exception handling will be applied globally or to a subset of controllers.


@ExceptionHandler and @ControllerAdvice are used to define a central point for treating exceptions and wrapping them up in a class.

You can also override the existing exception handlers. Spring Boot’s built-in exception class ResponseEntityExceptionHandler has multiple methods that you can override to customize the exception handling further.

Code Decode Playlists

Most Asked Core Java Interview Questions and Answers : https://youtube.com/playlist?list=PLy...

Advance Java Interview Questions and Answers : https://youtube.com/playlist?list=PLy...

Java 8 Interview Questions and Answers : https://youtube.com/playlist?list=PLy...

Hibernate Interview Questions and Answers : https://youtube.com/playlist?list=PLy...

Spring Boot Interview Questions and Answers : https://youtube.com/playlist?list=PLy...

Angular Playlist :  https://www.youtube.com/watch?v=CAl7R...

GIT : https://youtube.com/playlist?list=PLy...
