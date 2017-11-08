### Core Java

* **Explain OOP Concept**. _Abstraction_ means using simple things to reperesnt complexity. _Encapsulation \_this is the practice to keep the fields in class private then accessing them from a public function  \_Inheritance \_feature of OOP lets you share some of the attributes of exisiting classes. \_polymorphism. _**DRY \(Don’t Repeat Yourself\) / Single Responsibility / Open Closed Design. **

* **Differences between abstract classes and interfaces**? abstract class, unlike interfaces are classes. They are more expensive to use, becuase there is a look-up do when you inherit from them. an **interface **is a contract that have only the signature of the methods do not have body.

* **What is serialization?** **How do you implement it?** brake a class into byte code, used to pass objects between activities. better practice is to use Parcallable.

* **What is Singleton class**? a class that have only one instance.

* What is anonymous classes?

* **What is the difference between using**`==`**and**`.equals`**on a string?** the **==** compares memory address the equals method compares the objects.

* **What is the**`hashCode()`**and**`equals()`**used for?** HashCode returns an Integer to support the benefit of based collection classes such as Hashtable, HashMap, HashSet this method must be overriden in every calss that overrides the equals method. equals compare two objects

* **What are these**`final finally`**and**`finalize`? **final** class cannot be inherited, final method cant be overriden and final variable value cannot change. **finally** is used to place important code, its a block of code. **finalize** used to perform clean up processing just before object is garbage collected.

* **What is memory leak and how does Java handle it?**

* **What is garbage collector? How it works?**
* **Arrays vs ArrayLists **arrays are fixes in size ArrayList cannot create primitive data types.
* **HashSet vs TreeSet**  both do not hold duplicate items, **HashSet **performance \(faster\) than TreeSet for the operations like add, remove contains, size etc. **HashSet** offers constant time cost while TreeSet offers log\(n\) time cost for such operations.
* **Difference between method overloading and overriding. Ovlerloading** accurs when two or more methods in the class have the same method name but different params. **Overriding** means having two different methods with the same params but on a other child class.

* **What are the access modifiers you know? What does each one do? **private - helps encapsulate methods and vars. public - lets you access vars and classes

* **Can an Interface extend another Interface?** Yes.

* **What does the**`static`**word mean in Java? **static members belong to the class instead of a specific instance. it means only one instance of a static field exists. even if you create a miliion instance members. and static members can access instance members through an object reference.

* **Can a**`static`**method be overridden in Java? **No.

* **What is Polymorphism? What about Inheritance? **Polymorphism is where the method to be invoked is determined at runtime bae on the type of the object. polymorphism is a specific result of inheritance.

* **What is the difference between an Integer and int? **int is a primitive type

* **Do objects get passed by reference or value in Java? Elaborate on that. **java pass objects by references but don't pass method by reference. it passes them by value.

* **What is a ThreadPoolExecutor? **contains varying amount of threads, it's implemenation of the ExecutorService.
* **What the difference between local, instance and class variables? **
* **What is reflection?**
* **What are strong, soft and weak references in Java?**
* **What is dependency injection? Can you name few libraries? Have you used any?**
* **What does the keyword**`synchronized`**mean?**
* **What does it means to say that a**`String`**is immutable?**
* **What are**`transient`**and**`volatile`**modifiers**
* **What is the**`finalize()`**method?**
* **How does the**`try{}finally{}`**works? finally will get called any way**
* **What is the difference between instantiation and initialization of an object?**
* **When is a**`static`**block run?**
* **Explain Generics in Java?**
* **Difference between**`StringBuffer`**and**`StringBuilder`**?**
* **How is a**`StringBuilder`
  **implemented to avoid the immutable string allocation problem?**
* **What is Autoboxing and Unboxing?**
* **What’s the difference between an Enumeration and an Iterator?**
* **What is the difference between fail-fast and fail safe in Java?**
* **What is Java priority queue?**
* **What are the design patterns? **Design patterns are reusable solution to a commonly problem within a given context in software design. OOP design patterns typically show relationship and interaction between classes and objects.design patterns are grouped into these categories: creational patterns, structural patterns and behavioral patterns. The more known patterns are: _**Builder**_ \(Seperate the construction of a complex object from its representation\), _**Singleton**_ - Ensure a a class has only one instance and provide a global point of access to it. _**Factory method**_** **- Factory Method lets a a class defer instantiation to subclasses._** Decorator**_ - Attach additional responsibillities to an object dynamically keeping the same interface.  mainly to extend functionality. and there are many more. I wrote an example [project](/add) in Kotlin that shows many patterns.



