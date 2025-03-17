# OOP and Java Interview Questions & Answers

## 1. Why do we need to use OOP? Some major OOP languages?

OOP (Object-Oriented Programming) is needed because it promotes code reusability, modularity, and maintainability. It helps in organizing complex software projects by encapsulating data and behavior into objects. Some major OOP languages are Java, C++, Python, C#, and Ruby.  


## 2. Interface vs Abstract class?

- An **interface** only contains method declarations without implementations (except for default methods in Java 8+).  
- An **abstract class** can have both abstract (unimplemented) and concrete (implemented) methods.  
- A class can implement multiple interfaces but can inherit only one abstract class.  


## 3. Why do we need `equals` and `hashCode`? When to override?

- `equals()` is used to compare object values, while `==` checks reference equality.  
- `hashCode()` provides a unique integer for an object, mainly used in hash-based collections like HashMap.  
- Override them when working with objects stored in collections to ensure proper comparison and retrieval.  


## 4. Diamond problem in Java? How to fix it?

The diamond problem occurs when multiple inheritance leads to ambiguity in method resolution. In Java, it is avoided by allowing multiple interface inheritance but restricting multiple class inheritance. Default methods in interfaces can solve this issue by requiring explicit method overrides.  


## 5. Why do we need a Garbage Collector? How does it run?

Garbage Collector (GC) automatically reclaims memory occupied by objects that are no longer referenced. It prevents memory leaks and optimizes performance. It runs in the background, using algorithms like Mark-Sweep or Generational GC.  


## 6. Java ‘static’ keyword usage?

- Used to define class-level members (variables, methods, blocks).  
- `static` methods belong to the class, not an instance.  
- `static` blocks execute once when the class loads.  


## 7. Immutability means? Where, How and Why to use it?

Immutability means an object's state cannot be changed after creation. It is useful in multi-threading and caching. To create immutable objects, use `final` variables and avoid setters. Example: `String` in Java.  


## 8. Composition and Aggregation means and differences ?

- **Composition:** A strong relationship where the contained object cannot exist without the container. If the container is destroyed, the contained objects are also destroyed.
- **Aggregation:** A weaker relationship where the contained object can exist independently of the container. If the container is destroyed, the contained objects can still exist.


## 9. Cohesion and Coupling means and differences ?

- **Cohesion:** The degree to which elements within a module belong together. High cohesion is preferred as it improves maintainability and readability.
- **Coupling:** The degree of interdependence between modules. Low coupling is preferred to reduce dependencies and improve modularity.


## 10. Heap and Stack means and differences ?

- **Heap:** Used for dynamic memory allocation. Objects created using `new` are stored in the heap and managed by the Garbage Collector.
- **Stack:** Used for method execution and local variables. Each thread has its own stack, and variables are automatically removed when a method finishes execution.


## 11. Exception means ? Type of Exceptions ?

- **Exception:** An event that disrupts normal program execution.
- **Types of Exceptions:**
  - Checked Exceptions (e.g., IOException, SQLException)
  - Unchecked Exceptions (e.g., NullPointerException, ArrayIndexOutOfBoundsException)
  - Errors (e.g., OutOfMemoryError, StackOverflowError)


## 12. How to summarize ‘clean code’ as short as possible ?

"Clean code is readable, simple, and efficient. It follows best practices, avoids redundancy, and is easy to maintain."


## 13. What is the method of hiding in Java ?

- When a static method is defined in both parent and child classes with the same signature, the method in the child class hides the method in the parent class.
- Unlike method overriding, method hiding is specific to static methods.


## 14. What is the difference between abstraction and polymorphism in Java ?

- **Abstraction:** Hides implementation details and shows only relevant functionalities. Achieved using abstract classes and interfaces.
- **Polymorphism:** Allows a single interface to represent different data types or methods, making code more flexible and reusable.



