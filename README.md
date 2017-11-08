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

  1. One of HashMap's subclasses is[`LinkedHashMap`](http://java.sun.com/javase/7/docs/api/java/util/LinkedHashMap.html), so in the event that you'd want predictable iteration order \(which is insertion order by default\), you could easily swap out the[`HashMap`](http://java.sun.com/javase/7/docs/api/java/util/HashMap.html)for a[`LinkedHashMap`](http://java.sun.com/javase/7/docs/api/java/util/LinkedHashMap.html). This wouldn't be as easy if you were using[`Hashtable`](http://java.sun.com/javase/7/docs/api/java/util/Hashtable.html).

* **Breadth First Search**

* **Depth First Search**

* **Greedy Algorithm**

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
* **What are the design patterns?**

### Core Android

* **Explain activity lifecycle.** OnCreate -&gt; OnStart -&gt; OnResume -&gt; onPause -&gt; OnStop -&gt; OnDestroy
* **Tell all the Android appplication components. **Activities - dictate the UI, Services - Handle long running operations on the background , BroadCast Receivers - They handle communication between Android OS and applications, Content Providers -&gt; They handle data and database management issues.
* **Service vs IntentService. **The _Service \_can be used in tasks with no UI, but shouldn't be too long. If you need to perform long tasks, you must use threads within Service. The \_IntentService_  
  can be used in long tasks usually with no communication to Main Thread. If communication is required, can use Main Thread handler or broadcast intents. Another case of use is when callbacks are needed \(Intent triggered tasks\).

* **What is the structure of an Android Application? **Manifest, assets, resources, java classs

* **How to persist data in an Android app? **Shared Preferences, internal database like Realm, Room, SQLite, AndroidORM etc...

* **How would you perform a long-running operation in an application? **With a background Service.

* **How would you communicate between two Fragments? **Via interfaces throw the Activity that holds these Fragments

* **Explain Android notification system? ** A Notification is a message you display to the user outside of the app. to start getting notification you need to register the FCM service and listen to incoming messages. you show these notification with the NotificationManager.

* **How can two distinct Android apps interact? **You cannot access methods of another Activity in different apps. Broadcast would work but if you want more control consider binding to a remote service in the other app or use Messenger and handler to communicate.
* **What is Fragment? **A Fragment represents a behavoir of user interface in an Activity. you can combine multiple fragment in multiple activities. fragments have their own lifecycle.
* **Explain the lifecycle of a Fragment. **OnAttach -&gt; OnCreate -&gt; OnCreateView -&gt; onStart\(\) -&gt; onResume -&gt; onPause\(\) -&gt; onStop -&gt; onDestroyView -&gt; onDetach\(\) -&gt;
* **What is Dialog in Android? **There are ProgressDialogs, DialogFragments
* **What is View in Android? **View Objects are the basic building blocks of User Interface \(UI\) elements in Android. EditTextView, Button, CheckBox are childs of view.
* **Can you create custom views? How? **Yes, you can extend from LinearLayout, ReleativeLayout, FrameLayout etc to get their behavior and extend their functionality. 
* **What are ViewGroups and how they are different from the views? **A ViewGroup is a special view that can contain other views \(called children\).
* **What is the difference between a fragment and an activity? Explain the relationship between the two. **Activity is Android component that provides a screen, with which users can interact in. Whereas a Fragment reperesnt a behavior or portion of use interface in an Activity.
* **What is the difference between Serializable and Parcelable? Which is the best approach in Android? **In Android we know that we cannot pass objects in activities. The objects must be either implements serializable or Parcelable interface to do this. Serializable is a standard Java interface. You can just implement Serializable interface and add override methods.The problem with this approach is that reflection is used and it is a slow process. This method create a lot of temporary objects and cause quite a bit of garbage collection. Serializable interface is easier to implement.  Parcelable process is much faster than serializable. One of the reasons for this is that we are being explicit about the serialization process instead of using reflection to infer it. It also stands to reason that the code has been heavily optimized for this purpose.
* **What are "launch modes"? **Activities live in a stack that contains a collection of activity instances. Launch mode allows you to define how a new instance or the exiting instance of an activity is associated with the current task. the activity launch mode has four valid values that you can control in the Manifest file. _**Standard** - _This is the common mode for most of the activities. Multiple instances of the activity calss can be instantiated and multiple instances can be added to the same task or different tasks. _**singleTop** -_ if an instance of activity already exists at the top of the current task and system routes intent to this activity, no new instance will be created becuse it will fire off an onNewIntent. _**SingleTask - **_A new task will always be created and a new instance will be pushed to the task as the root one. However, if any activity instance exists in any tasks, the system routes the intent to that activity instance through onNewIntent\(\). _**SingleInstance **_Same as SingleTask, except that the no activities instance can be pushed into the same task of the singleInstance's. That means, the activity with launch mode is always in a single activity instance task. this is a very specialized mode and should only be used in the applications taht are implemented entirely as one activity

```
<activity android:launchMode = ["standard" | "singleTop" | "singleTask" | "singleInstance"] ../> 
```

*  ‘standard’ and ‘singleTop’ can instantiate multiple activity instances and the instance will stay in the same task.
* For ‘singleTask’ or ‘singleInstance’, the activity class uses the singleton pattern, and that instance will be the root activity of a new task. Let’s examine each value:

* **What are Intents? **an "intention" to perform an action, basically a message to say you did or want something to happen. must of the time it used to navigate between activities. the user can "payload" to it called Bundle. 
* **What is an Implicit Intent?**
* **What is an Explicit Intent?**
* **What is an AsyncTask?**
* **What is a BroadcastReceiver?**
* **What is DDMS and what can you do with it?**
* **What is the support library? Why was it introduced?**
* **What is a ContentProvider and what is it typically used for?**
* **What is ADB?**
* **What is ANR? How can the ANR be prevented?**
* **What is AndroidManifest.xml?**
* **Describe how broadcasts and intents work to be able to pass messages around your app?**
* **How do you handle Bitmaps in Android as it takes too much memory?**
* **What are different ways to store data in your Android app?**
* **What is the Dalvik Virtual Machine?**
* **What is the relationship between the life cycle of an AsyncTask and an Activity? What problems can this result in? How can these problems be avoided?**
* **What is the function of an intent filter?**
* **What is a Sticky Intent?**
* **What is AIDL? Enumerate the steps in creating a bounded service through AIDL.**
* **What are the different protection levels in permission?**
* **How would you preserve Activity state during a screen rotation?**
* **Relative Layout vs Linear Layout.**
* **How to implement XML namespaces?**
* **Difference between View.GONE and View.INVISIBLE?**
* **What is the difference between a regular bitmap and a nine-patch image?**
* **Tell about the bitmap pool.**
* **How to avoid memory leaks in Android?**
* **What are widgets on Home-Screen in Android?**
* **What is AAPT?**
* **How do you find memory leaks in Android applications?**
* **How do you troubleshoot a crashing application?**
* **Why should you avoid to run non-ui code on the main thread?**
* **How did you support different types of resolutions?**
* **What is Doze? What about App Standby?**
* **What can you use for background processing in Android?**
* **What is ORM? How does it work?**
* **What is a Loader?**
* **What is the NDK and why is it useful?**
* **What is the StrictMode?**
* **What is Lint? What is it used for?**
* **What is a SurfaceView?**
* **What is the difference between ListView and RecyclerView?**
* **What is the ViewHolder pattern? Why should we use it?**
* **What is a PendingIntent?**
* **Can you manually call the Garbage collector?**
* **What is the best way to update the screen periodically?**
* **What are the different types of Broadcasts?**
* **Have you developed widgets? Describe.**
* **What is Context? How is it used?**
* **Do you know what is the view tree? How can you optimize its depth?**
* **What is the**`onTrimMemory`
  **method?**
* **Is it possible to run an Android app in multiple processes? How?**
* **How does the OutOfMemory happens?**
* **What is a**`spannable`**?**
* **What is renderscript?**
* **What are the differences between Dalvik and ART?**
* **FlatBuffers vs JSON.**
* **What are Annotations**
* **Tell about Constraint Layout**
* **HashMap, ArrayMap and SparseArray**
* **Explain Looper, Handler and HandlerThread.**
* **How to reduce battery usage in an android application?**
* **What is**`SnapHelper`**?**

### Architecture

* **Describe the architecture of your last app.**
* **Describe MVP.**
* **What is presenter?**
* **What is model?**
* **Describe MVC.**
* **What is controller?**
* **Describe MVVM.**
* **Tell something about clean code**

### Design Problem

* **Design Uber App.**
* **Design Facebook App.**
* **Design Facebook Near-By Friends App.**
* **Design WhatsApp.**
* **Design SnapChat.**
* **Design problems based on location based app.**

### Tools And Technologies

* **Git.**
* **RxJava.**
* **Dagger 2 **
* **Android Development Useful Tools.**

### Android Test Driven Development

* **What is Espresso?**
* **What is Robolectric?**
* **What is UI-Automator?**
* **Explain unit test.**
* **Explain instrumented test.**
* **Have you done unit testing or automatic testing?**
* **Why Mockito is used? \[Link\]**
* **Describe JUnit test.**

### Advanced

* **Describe how REST APIs work.**
* **Describe SQLite.**
* **Describe database.**
* **Project Management tool - trello, basecamp, kanban, jira, asana.**
* **About build System - gradle, ant, buck.**
* **Reverse Engineering an APK.**
* **What is proguard used for?**
* **What is obfuscation? What is it used for? What about minification?**
* **How do you build your apps for release?**
* **APK Size Reduction.**
* **Android Development Best Practices.**
* **Android Code Style And Guidelines.**

* **Have you tried Kotlin?**

* **What are the metrics that you should measure continuously while android application development?**



