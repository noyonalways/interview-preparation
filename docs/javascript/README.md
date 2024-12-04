![JavaScript Banner](https://via.placeholder.com/1200x300.png?text=JavaScript)

# JavaScript

- [JavaScript](#javascript)
  - [1. What is the Higher Order function \& callback function in JavaScript?](#1-what-is-the-higher-order-function--callback-function-in-javascript)
  - [2. What is Hoisting in JavaScript?](#2-what-is-hoisting-in-javascript)
  - [3. What is Scope in JavaScript?](#3-what-is-scope-in-javascript)
  - [4. What is the difference between Call, Apply and Bind?](#4-what-is-the-difference-between-call-apply-and-bind)
  - [5. What is the difference between `==` and `===` operators?](#5-what-is-the-difference-between--and--operators)
  - [6. What is a cookie?](#6-what-is-a-cookie)
  - [7. What is a promise?](#7-what-is-a-promise)
  - [8. What is an event loop?](#8-what-is-an-event-loop)
  - [9. What is a prototype chain?](#9-what-is-a-prototype-chain)
  - [10. How can you eliminate the duplicate values from a JavaScript array?](#10-how-can-you-eliminate-the-duplicate-values-from-a-javascript-array)

### 1. What is the Higher Order function & callback function in JavaScript?

A higher-order function is a function that accepts one or more functions as arguments or returns a function as a return value or both.
A Callback function is a function that is passed as an argument to another function and is executed after the completion of some operation. Callbacks are commonly used to perform asynchronous functions such as data fetching, event handling, and other time-consuming operations.

### 2. What is Hoisting in JavaScript?

Hoisting is a concept or behavior in JavaScript where the declaration variable, function, or class goes to the top of the scope during the compilation phase before the code is executed. Hoisting moves declarations to the top, but not their values.

### 3. What is Scope in JavaScript?

In JavaScript, scope refers to accessing variables, objects, and functions from different parts of the code.

JavaScript offers various types of scope, the primary ones being global, local, and block scope. These scopes control the accessibility of variables in different parts of our code and play a pivotal role in maintaining code organizing and preventing variable conflicts.

### 4. What is the difference between Call, Apply and Bind?

In JavaScript, at a very level call and apply execute a function immediately. bind returns a new function.

Call and apply are very similar in that they allow you to invoke a function. The difference is that call takes arguments one by one, and apply takes in arguments as an array.

Bind is used to return a function that can be invoked at a later time. The bind() method creates a new function that, when called, has its this keyword set to the provided value, with a given sequence of arguments preceding any provided when the new function is called.

Call: The call() method invokes a function with a given this value and arguments provided one by one.
Apply: Invokes the function with a given this value and allows us to pass in arguments as an array.
Bind: returns a new function, allowing us to pass any number of arguments

### 5. What is the difference between `==` and `===` operators?

JavaScript provides both strict `===` and type-converting `==` equality comparison. The strict operator takes the type of variable into
consideration, while the non-strict operator makes type correction/conversion based on the values of variables.

### 6. What is a cookie?

Cookies are small files of information that a web server generates and sends to a web browser. Web browsers store the cookies they receive for a predetermined period, or the length of a user's session on a website. They attach the relevant cookies to any future requests the user makes to the web server.

Cookies help inform websites about the user, enabling the websites to personalize the user experience.

### 7. What is a promise?

A promise in JavaScript is like a container for a future value. It is a way of saying, “I don’t have this value right now, but I will have it later.” For example, I order a book online. I don’t get the book right away, but the store promises to send it to me. While I wait, I can do other things, and when the book arrives, I can read it.

In the same way, a promise lets us keep working with our code while waiting for something else to finish, like loading data from a server. When the data is ready, the promise will deliver it.

A promise can be in one of three states:
Pending: The promise is waiting for something to finish. For example, waiting for data to load from a website.
Fulfilled: The promise has been completed successfully. The data I was waiting for is now available.
Rejected: The promise has failed. Maybe there was a problem, like the server not responding.

### 8. What is an event loop?

The event loop is a process that continuously monitors the call stack and the event queue and checks whether or not the call stack is empty. If the call stack is empty and there are pending events in the event queue, the event loop dequeues the event from the event queue and pushes it to the call stack. The call stack executes the event and any additional events generated during the execution are added to the end of the event queue.

The event loop allows Node.js to perform non-blocking I/O operations, even though JavaScript is single-threaded, by offloading operations to the system kernel whenever possible. Since most modern kernels are multi-threaded, they can handle multiple operations executing in the background.

### 9. What is a prototype chain?

Prototype chaining is a feature in JavaScript that allows objects to inherit properties and methods from other objects. It is a key aspect of the language's prototype-based inheritance model. In JavaScript, every object has a prototype, which is another object from which it inherits properties and methods. This chain of prototypes forms what is known as the prototype chain.

### 10. How can you eliminate the duplicate values from a JavaScript array?

To eliminate duplicate values from a JavaScript array, we can use several techniques depending on our preference or the complexity of the task. The most common ways

- Using Set
- Using filter and indexOf
- Using reduce
- Using forEach and a Set or Object
