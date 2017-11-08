### Data Structures And Algorithms

> The level of questions asked on Data Structures And Algorithms totally depends on the company for which you are applying.

* **ArrayList** -  Resizable-array implementation of List interface. 
* **LinkedList** can contain duplicate elements, maintains insertion order,
* **DoublyLinkedList** - each node contains tow fields called _links, \_that are references to the previous_ and to the \_next node, when deleting a node the previous one getting deleted
* **Stack **The Stack calss reperesent a last-in-first-out \(LIFO\) stack of objects. It extends the class Vector with five operation that allow vector to be treated as a stack.Modifier and Type
  |  | Method and Description |
  | :--- | :--- |
  | `boolean` | [`empty`](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html#empty%28%29)`()`Tests if this stack is empty. |
  | [`E`](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html) | [`peek`](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html#peek%28%29)`()`Looks at the object at the top of this stack without removing it from the stack. |
  | [`E`](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html) | [`pop`](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html#pop%28%29)`()`Removes the object at the top of this stack and returns that object as the value of this function. |
  | [`E`](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html) | [`push`](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html#push%28E%29)`(`[`E`](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html)`item)`Pushes an item onto the top of this stack. |
  | `int` | [`search`](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html#search%28java.lang.Object%29)`(`[`Object`](https://docs.oracle.com/javase/7/docs/api/java/lang/Object.html)`o)`Returns the 1-based position where an object is on this stack. |
* **Queue FIFO - **peek\(\) will retrieve the object but will not remove it, add\(\) will insert, poll\(\) will retrieve and remove the elemnt
* **PriorityQueue - **he elements of the priority queue are ordered according to their natural ordering
* **Dynamic** **Programming **must of the time used for optimization. a dynamic programming algo will will examine the previously solved problam and will combine their solutions to give the best solution for the given problem
* **String Manipulation **
* **Binary Tree **its a tree which each node has at most two children, which are referred to as the _left_ _child _ and the _right child. _
* **Binary Search Tree **it's like a binary tree but they allow fast lookup. Binary search trees keep their keys in sorted order, support three main operations: insertion of element, deletion of elements, lookup.
* **Sorting Algorithms **Quick Sort - 
* **Hash Table or Hash Map **[`Hashtable`](http://java.sun.com/javase/7/docs/api/java/util/Hashtable.html)is [synchronized](https://stackoverflow.com/questions/1085709/what-does-synchronized-mean), whereas[`HashMap`](http://java.sun.com/javase/7/docs/api/java/util/HashMap.html)is not. This makes[`HashMap`](http://java.sun.com/javase/7/docs/api/java/util/HashMap.html)better for non-threaded applications, as unsynchronized Objects typically perform better than synchronized ones.
  1. [`Hashtable`](http://java.sun.com/javase/7/docs/api/java/util/Hashtable.html)does not allow`null`keys or values.[`HashMap`](http://java.sun.com/javase/7/docs/api/java/util/HashMap.html)allows one`null`key and any number of`null`values.

  2. One of HashMap's subclasses is[`LinkedHashMap`](http://java.sun.com/javase/7/docs/api/java/util/LinkedHashMap.html), so in the event that you'd want predictable iteration order \(which is insertion order by default\), you could easily swap out the[`HashMap`](http://java.sun.com/javase/7/docs/api/java/util/HashMap.html)for a[`LinkedHashMap`](http://java.sun.com/javase/7/docs/api/java/util/LinkedHashMap.html). This wouldn't be as easy if you were using[`Hashtable`](http://java.sun.com/javase/7/docs/api/java/util/Hashtable.html).
* **Breadth First Search**
* **Depth First Search**
* **Greedy Algorithm**

### Core Java

* **Explain OOP Concept**. _Abstraction_ means using simple things to reperesnt complexity. _Encapsulation _this is the practice to keep the fields in class private then accessing them from a public function  _Inheritance _feature of OOP lets you share some of the attributes of exisiting classes. _polymorphism. _**DRY \(Don’t Repeat Yourself\) / Single Responsibility / Open Closed Design. **

* **Differences between abstract classes and interfaces**? abstract class, unlike interfaces are classes. They are more expensive to use, becuase there is a look-up do when you inherit from them. an **interface **is a contract that have only the signature of the methods do not have body.
* **What is serialization?** How do you implement it? brake a class into byte code, used to pass objects between activities. better practice is to use Parcallable. 
* **What is Singleton class**? a class that have only one instance.
* What is anonymous classes? 
* **What is the difference between using`==`and`.equals`on a string?** the **==** compares memory address the equals method compares the objects.
* **What is the`hashCode()`and`equals()`used for?** HashCode returns an Integer to support the benefit of based collection classes such as Hashtable, HashMap, HashSet this method must be overriden in every calss that overrides the equals method. equals compare two objects 
* **What are these`final finally`and`finalize`**? **final** class cannot be inherited, final method cant be overriden and final variable value cannot change. **finally** is used to place important code, its a block of code. **finalize** used to perform clean up processing just before object is garbage collected.
* **What is memory leak and how does Java handle it?** 
* What is garbage collector? How it works?
* **Arrays vs ArrayLists **arrays are fixes in size ArrayList cannot create primitive data types.
* **HashSet vs TreeSet**  both do not hold duplicate items, **HashSet **performance \(faster\) than TreeSet for the operations like add, remove contains, size etc. **HashSet** offers constant time cost while TreeSet offers log\(n\) time cost for such operations.
* Typecast in Java. with the TreeSet the elements will be sorted.
* Difference between method overloading and overriding.
* What are the access modifiers you know? What does each one do?
* Can an Interface extend another Interface?
* What does the`static`word mean in Java?
* Can a`static`method be overridden in Java?
* What is Polymorphism? What about Inheritance?
* What is the difference between an Integer and int?
* Do objects get passed by reference or value in Java? Elaborate on that.
* What is a ThreadPoolExecutor?
* What the difference between local, instance and class variables?
* What is reflection?
* What are strong, soft and weak references in Java?
* What is dependency injection? Can you name few libraries? Have you used any?
* What does the keyword`synchronized`mean?
* What does it means to say that a`String`is immutable?
* What are`transient`and`volatile`modifiers
* What is the`finalize()`method?
* **How does the`try{}finally{}`works? **finally will get called any way
* What is the difference between instantiation and initialization of an object?
* When is a`static`block run?
* Explain Generics in Java?
* Difference between`StringBuffer`and`StringBuilder`?
* How is a`StringBuilder`
  implemented to avoid the immutable string allocation problem?
* What is Autoboxing and Unboxing?
* What’s the difference between an Enumeration and an Iterator?
* What is the difference between fail-fast and fail safe in Java?
* What is Java priority queue?
* What are the design patterns?
  [Link](https://github.com/iluwatar/java-design-patterns)

### Core Android

* Explain activity lifecycle.
* Tell all the Android appplication components.
* Service vs IntentService.
* What is the structure of an Android Application?
* How to persist data in an Android app?
* How would you perform a long-running operation in an application?
* How would you communicate between two Fragments?
* Explain Android notification system?
* How can two distinct Android apps interact?
* What is Fragment?
* Explain the lifecycle of a Fragment.
* What is Dialog in Android?
* What is View in Android?
* Can you create custom views? How?
* What are ViewGroups and how they are different from the views?
* What is the difference between a fragment and an activity? Explain the relationship between the two.
* What is the difference between Serializable and Parcelable? Which is the best approach in Android?
* What are "launch modes"?
* What are Intents?
* What is an Implicit Intent?
* What is an Explicit Intent?
* What is an AsyncTask?
* What is a BroadcastReceiver?
* What is DDMS and what can you do with it?
* What is the support library? Why was it introduced?
* What is a ContentProvider and what is it typically used for?
* What is ADB?
* What is ANR? How can the ANR be prevented?
* What is AndroidManifest.xml?
* Describe how broadcasts and intents work to be able to pass messages around your app?
* How do you handle Bitmaps in Android as it takes too much memory?
* What are different ways to store data in your Android app?
* What is the Dalvik Virtual Machine?
* What is the relationship between the life cycle of an AsyncTask and an Activity? What problems can this result in? How can these problems be avoided?
* What is the function of an intent filter?
* What is a Sticky Intent?
* What is AIDL? Enumerate the steps in creating a bounded service through AIDL.
* What are the different protection levels in permission?
* How would you preserve Activity state during a screen rotation?
* Relative Layout vs Linear Layout.
* How to implement XML namespaces?
* Difference between View.GONE and View.INVISIBLE?
* What is the difference between a regular bitmap and a nine-patch image?
* Tell about the bitmap pool.
* How to avoid memory leaks in Android?
* What are widgets on Home-Screen in Android?
* What is AAPT?
* How do you find memory leaks in Android applications?
* How do you troubleshoot a crashing application?
* Why should you avoid to run non-ui code on the main thread?
* How did you support different types of resolutions?
* What is Doze? What about App Standby?
* What can you use for background processing in Android?
* What is ORM? How does it work?
* What is a Loader?
* What is the NDK and why is it useful?
* What is the StrictMode?
* What is Lint? What is it used for?
* What is a SurfaceView?
* What is the difference between ListView and RecyclerView?
* What is the ViewHolder pattern? Why should we use it?
* What is a PendingIntent?
* Can you manually call the Garbage collector?
* What is the best way to update the screen periodically?
* What are the different types of Broadcasts?
* Have you developed widgets? Describe.
* What is Context? How is it used?
* Do you know what is the view tree? How can you optimize its depth?
* What is the`onTrimMemory`
  method?
* Is it possible to run an Android app in multiple processes? How?
* How does the OutOfMemory happens?
* What is a`spannable`?
* What is renderscript?
* What are the differences between Dalvik and ART?
* FlatBuffers vs JSON.
* What are Annotations
* Tell about Constraint Layout
* HashMap, ArrayMap and SparseArray
* Explain Looper, Handler and HandlerThread.
* How to reduce battery usage in an android application?
* What is`SnapHelper`?

### Architecture

* Describe the architecture of your last app.
* Describe MVP.
* What is presenter?
* What is model?
* Describe MVC.
* What is controller?
* Describe MVVM.
* Tell something about clean code

### Design Problem

* Design Uber App.
* Design Facebook App.
* Design Facebook Near-By Friends App.
* Design WhatsApp.
* Design SnapChat.
* Design problems based on location based app.

### Tools And Technologies

* Git.
* RxJava.
* Dagger 2 
* Android Development Useful Tools.

### Android Test Driven Development

* What is Espresso?
* What is Robolectric?
* What is UI-Automator?
* Explain unit test.
* Explain instrumented test.
* Have you done unit testing or automatic testing?
* Why Mockito is used? \[Link\]
* Describe JUnit test.

### Others

* Describe how REST APIs work.
* Describe SQLite.
* Describe database.
* Project Management tool - trello, basecamp, kanban, jira, asana.
* About build System - gradle, ant, buck.
* Reverse Engineering an APK.
* What is proguard used for?
* What is obfuscation? What is it used for? What about minification?
* How do you build your apps for release?
* APK Size Reduction.
* Android Development Best Practices.
* Android Code Style And Guidelines.

* Have you tried Kotlin?

* What are the metrics that you should measure continuously while android application development?



