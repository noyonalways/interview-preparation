![TypeScript Banner](https://via.placeholder.com/1200x300.png?text=TypeScript)

# TypeScript

### 1. What are the three main primitive data types in TypeScript?

The three main primitive data types in TypeScript. These are

- **String**: Represents textual data
- **Number**: Represents numeric values, including integers and floating-point numbers
- **Boolean**: Represents true or false values.

### 2. What is an interface in TypeScript?

Interface is a feature of TypeScript that allows us to define the structure or shape of an object and specify the properties and methods that an object has or should have. Interfaces ar primarily used for type-checking and ensuring that an object adheres to a particular structure.
Key features of interfaces:

- **Defining Object structure**
- **Optional properties**
- **Function type definitions**
- **Extending interfaces**
- **Read-only properties**

### 3. What is a type assertion in TypeScript?

In TypeScript, Type assertion is a technique that explicitly tells the TypeScript compiler about the type of a value. It essentially overrides the compiler’s inferred type, allowing us to specify a more specific or compatible type.
Type assertions are useful when we know about the type of a value that TypeScript can infer, such as when working with dynamic data or third-party libraries.
There are two ways to perform a type assertion:

- `< >` angle-bracket Syntax
- `as` Syntax

### 4. How many access modifiers are there in TypeScript?

TypeScript provides three access modifiers used to control the visibility of class members (properties and methods).

- `public`
- `private`
- `protected`

### 5. What are getters/setters?

In TypeScript, there are two supported methods getter and setter to access and set the class members. Getters and setters are nothing but a way for us to provide access to the properties of an object. Unlike other OOP languages like Java, C++, etc. Where we can only access variables via the getter or setter method, things work differently in TypeScript where we can access variables directly.
For each property:

- A getter method returns the value of the property’s value. A getter is also called an accessor.
- A setter method updates the property’s value. A setter is also known as a mutator.

### 6. How do you define a type alias in TypeScript? & Explain the purpose of type aliases in TypScript.

In TypeScript, a type alias allows us to create a custom name for a type, making our code more readable and reusable. We use the type keyword to define it.
Purpose of Type aliases in TypeScript:

- **Simplify complex types:** Type aliases make it easier to work with long or repetitive types.
- **Increase readability:** Provide meaningful names to types for better understanding.
- **Reusable types:** Use the same alias in multiple places to reduce duplication.
- **Dynamic Union and Intersection types:** Easily define combinations of types.

### 7. What is the difference between public, private, and protected access modifiers?

- **public:** The public modifier allows class properties and methods to be accessible from all locations. If we don’t specify any access modifier for properties and methods, they will take the public modifier by default.
- **private:** The private modifier limits the visibility to the same class only. When we add the private modifier to a property or method, we can access that property or method within the same class. Any attempt to access private properties or methods outside the class will result in an error at complied time.
- **protected:** The protected modifier allows properties and methods of a class to be accessible within the same class and subclasses. When a class (child class) inherits from another class (parent class) it is a subclass of the parent class.

### 8. Describe the difference between any and unknown types in TypeScript. When would you use each?

In TypeScript there are two special types: any and unknown. Both provide flexibility in TypeScript's type system and offer a way to bypass TypeScript’s type checking. At a glance, any and unknown seem to be similar, however, their behaviors differ significantly.

- **any:** The any type tells the compiler to trust us about the type of a variable and doesn’t enforce type checks during compilation. A variable of type any behaves like a regular JavaScript variable, it can be freely reassigned or used in any context without restrictions.
- **unknown:** Introduced in TypeScript 3.0, unknown is the more type-safe counterpart of any. While it represents any value (just like any), TypeScript will ensure that we check the type of the variable before using it. This ensures better type safety and prevents runtime errors

### 9. How do you handle null and undefined in TypeScript?

Handling null and undefined in TypeScript ensures our code is safe and avoids runtime errors. Here’s how to deal with them:
Enable strictNullChecks: to treat null and undefined as separate types for better type safety.

- **Use union types:** Explicitly allow null or undefined in the variable’s type.
- **Default values (??):** Provide a fallback value when the variable is null or undefined.
- **Optional Chaining (?.):** Safely access properties that might be null or undefined.
- **Type Guard:** Checks if a value is not null or undefined before using it.
- **Non-Null Assertion (!):** Use ! when we are sure a value isn’t null or undefined.

### 10. Describe the difference between interface and type in TypeScript.

In TypeScript, both types and interfaces serve a similar purpose, they allow us to define the shape of data. However, there are some differences between them.

- **Type:** A type in TypeScript is like a label that can apply to any value. It allows us to define custom types that can be used throughout our code. Types are very flexible and can represent a wide range of data structures, including primitive types like numbers and strings, as well as more complex structures like objects and arrays
- **Interface:** On the other hand, an interface is a way to define the shape of an object. It allows us to specify the properties and their types that an object must have. Interfaces often enforce a contract between different parts of our code, ensuring that objects have the correct structure.
