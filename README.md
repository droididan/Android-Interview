### Data Structures And Algorithms

> The level of questions asked on Data Structures And Algorithms totally depends on the company for which you are applying.

* **ArrayList** -  Resizable-array implementation of List interface. 
* **LinkedList** can contain duplicate elements, maintains insertion order,
* **DoublyLinkedList** - each node contains tow fields called _links, \_that are references to the previous_ and to the \_next node, when deleting a node the previous one getting deleted
* **Stack **The Stack calss reperesent a last-in-first-out \(LIFO\) stack of objects. It extends the class Vector with five operation that allow vector to be treated as a stack.Modifier and Type
  |  | Method and Description |
  | :--- | :--- |
  | `boolean` | [**`empty`**](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html#empty%28%29)`()`Tests if this stack is empty. |
  | [`E`](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html) | [**`peek`**](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html#peek%28%29)`()`Looks at the object at the top of this stack without removing it from the stack. |
  | [`E`](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html) | [**`pop`**](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html#pop%28%29)`()`Removes the object at the top of this stack and returns that object as the value of this function. |
  | [`E`](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html) | [**`push`**](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html#push%28E%29)`(`[`E`](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html)` item)`Pushes an item onto the top of this stack. |
  | `int` | [**`search`**](https://docs.oracle.com/javase/7/docs/api/java/util/Stack.html#search%28java.lang.Object%29)`(`[`Object`](https://docs.oracle.com/javase/7/docs/api/java/lang/Object.html)` o)`Returns the 1-based position where an object is on this stack. |
* **Queue FIFO - **peek\(\) will retrieve the object but will not remove it, add\(\) will insert, poll\(\)
* **PriorityQueue**
* **Dynamic** **Programming**
* **String Manipulation**
* **Binary Tree**
* **Binary Search Tree**
* **Sorting Algorithms**
* **Hash Table or Hash Map**
* **Breadth First Search**
* **Depth First Search**
* **Greedy Algorithm**

### Core Java

* Explain OOP Concept.
* Differences between abstract classes and interfaces?
* What is serialization? How do you implement it?
* What is Singleton class?
* What is anonymous classes?
* What is the difference between using
  `==`
  and
  `.equals`
  on a string?
* What is the
  `hashCode()`
  and
  `equals()`
  used for?
* What are these
  `final`
  ,
  `finally`
  and
  `finalize`
  ?
* What is memory leak and how does Java handle it?
* What is garbage collector? How it works?
* Arrays vs ArrayLists.
* HashSet vs TreeSet.
* Typecast in Java.
* Difference between method overloading and overriding.
* What are the access modifiers you know? What does each one do?
* Can an Interface extend another Interface?
* What does the
  `static`
  word mean in Java?
* Can a
  `static`
  method be overridden in Java?
* What is Polymorphism? What about Inheritance?
* What is the difference between an Integer and int?
* Do objects get passed by reference or value in Java? Elaborate on that.
* What is a ThreadPoolExecutor?
  [Link](https://blog.mindorks.com/threadpoolexecutor-in-android-8e9d22330ee3)
* What the difference between local, instance and class variables?
* What is reflection?
* What are strong, soft and weak references in Java?
* What is dependency injection? Can you name few libraries? Have you used any?
* What does the keyword
  `synchronized`
  mean?
* What does it means to say that a
  `String`
  is immutable?
* What are
  `transient`
  and
  `volatile`
  modifiers?
* What is the
  `finalize()`
  method?
* How does the
  `try{}finally{}`
  works?
* What is the difference between instantiation and initialization of an object?
* When is a
  `static`
  block run?
* Explain Generics in Java?
* Difference between
  `StringBuffer`
  and
  `StringBuilder`
  ?
* How is a
  `StringBuilder`
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
  [Link](https://blog.mindorks.com/android-activity-launchmode-explained-cbc6cf996802)
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
  [Link](https://blog.mindorks.com/how-to-use-bitmap-pool-in-android-56c71a55533c)
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
  [Link](https://blog.mindorks.com/use-strictmode-to-find-things-you-did-by-accident-in-android-development-4cf0e7c8d997)
* What is Lint? What is it used for?
* What is a SurfaceView?
* What is the difference between ListView and RecyclerView?
* What is the ViewHolder pattern? Why should we use it?
* What is a PendingIntent?
* Can you manually call the Garbage collector?
* What is the best way to update the screen periodically?
* What are the different types of Broadcasts?
* Have you developed widgets? Describe.
  [Link](https://blog.mindorks.com/android-widgets-ad3d166458d3)
* What is Context? How is it used?
  [Link](https://medium.com/p/understanding-context-in-android-application-330913e32514)
* Do you know what is the view tree? How can you optimize its depth?
* What is the
  `onTrimMemory`
  method?
* Is it possible to run an Android app in multiple processes? How?
* How does the OutOfMemory happens?
* What is a
  `spannable`
  ?
* What is renderscript?
  [Link](https://blog.mindorks.com/comparing-android-ndk-and-renderscript-1a718c01f6fe)
* What are the differences between Dalvik and ART?
* FlatBuffers vs JSON.
  [Link](https://blog.mindorks.com/why-consider-flatbuffer-over-json-2e4aa8d4ed07)
* What are Annotations?
  [Link](https://blog.mindorks.com/creating-custom-annotations-in-android-a855c5b43ed9)
  ,
  [Link](https://blog.mindorks.com/improve-your-android-coding-through-annotations-26b3273c137a)
* Tell about Constraint Layout
  [Link](https://blog.mindorks.com/using-constraint-layout-in-android-531e68019cd)
* HashMap, ArrayMap and SparseArray
  [Link](https://blog.mindorks.com/android-app-optimization-using-arraymap-and-sparsearray-f2b4e2e3dc47)
* Explain Looper, Handler and HandlerThread.
  [Link](https://blog.mindorks.com/android-core-looper-handler-and-handlerthread-bd54d69fe91a)
* How to reduce battery usage in an android application?
  [Link](https://blog.mindorks.com/battery-optimization-for-android-apps-f4ef6170ff70)
* What is
  `SnapHelper`
  ?
  [Link](https://blog.mindorks.com/using-snaphelper-in-recyclerview-fc616b6833e8)

### Architecture

* Describe the architecture of your last app.
* Describe MVP.
  [Link](https://blog.mindorks.com/essential-guide-for-designing-your-android-app-architecture-mvp-part-1-74efaf1cda40)
* What is presenter?
* What is model?
* Describe MVC.
* What is controller?
* Describe MVVM.
  [Link](https://github.com/MindorksOpenSource/android-mvvm-architecture)
* Tell something about clean code
  [Link](https://blog.mindorks.com/every-programmer-should-read-this-book-6755dedec78d)

### Design Problem

* Design Uber App.
* Design Facebook App.
* Design Facebook Near-By Friends App.
* Design WhatsApp.
* Design SnapChat.
* Design problems based on location based app.

### Tools And Technologies

* Git.
  [Link](https://github.com/git-tips/tips)
* RxJava.
  [Link](https://blog.mindorks.com/a-complete-guide-to-learn-rxjava-b55c0cea3631)
* Dagger 2.
  [Link](https://medium.com/p/a-complete-guide-to-learn-dagger-2-b4c7a570d99c)
* Android Development Useful Tools.
  [Link](https://blog.mindorks.com/android-development-useful-tools-fd73283e82e3)

### Android Test Driven Development

* What is Espresso?
  [Link](https://developer.android.com/training/testing/ui-testing/espresso-testing.html)
* What is Robolectric?
  [Link](http://robolectric.org/)
* What is UI-Automator?
  [Link](https://developer.android.com/training/testing/ui-testing/uiautomator-testing.html)
* Explain unit test.
* Explain instrumented test.
* Have you done unit testing or automatic testing?
* Why Mockito is used? \[Link\] \(
  [http://site.mockito.org/](http://site.mockito.org/)
  \)
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
  [Link](https://blog.mindorks.com/how-i-decreased-my-app-size-to-70-using-apk-analyser-4a6f79512072)
* Android Development Best Practices.
  [Link](https://blog.mindorks.com/android-development-best-practices-83c94b027fd3)
* Android Code Style And Guidelines.
  [Link](https://blog.mindorks.com/android-code-style-and-guidelines-d5f80453d5c7)
* Have you tried Kotlin?
  [Link](https://medium.com/p/why-you-must-try-kotlin-for-android-development-e14d00c8084b)
* What are the metrics that you should measure continuously while android application development?
  [Link](https://blog.mindorks.com/android-app-performance-metrics-a1176334186e)



