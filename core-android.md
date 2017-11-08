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

* **What are "launch modes"? **Activities live in a stack that contains a collection of activity instances. Launch mode allows you to define how a new instance or the exiting instance of an activity is associated with the current task. the activity launch mode has four valid values that you can control in the Manifest file. _**Standard** - \_This is the common mode for most of the activities. Multiple instances of the activity calss can be instantiated and multiple instances can be added to the same task or different tasks. _**singleTop** -_ if an instance of activity already exists at the top of the current task and system routes intent to this activity, no new instance will be created becuse it will fire off an onNewIntent. _**SingleTask - **_A new task will always be created and a new instance will be pushed to the task as the root one. However, if any activity instance exists in any tasks, the system routes the intent to that activity instance through onNewIntent\(\). _**SingleInstance **\_Same as SingleTask, except that the no activities instance can be pushed into the same task of the singleInstance's. That means, the activity with launch mode is always in a single activity instance task. this is a very specialized mode and should only be used in the applications taht are implemented entirely as one activity

```
<activity android:launchMode = ["standard" | "singleTop" | "singleTask" | "singleInstance"] ../>
```

* ‘standard’ and ‘singleTop’ can instantiate multiple activity instances and the instance will stay in the same task.
* For ‘singleTask’ or ‘singleInstance’, the activity class uses the singleton pattern, and that instance will be the root activity of a new task. Let’s examine each value:

* **What are Intents? **an "intention" to perform an action, basically a message to say you did or want something to happen. must of the time it used to navigate between activities. the user can "payload" to it called Bundle.

* **What is an Implicit Intent? **Implicit Intents do not directly specify the Android components which should be called , it only specifies action to be performed. for example open Google Map or sending an email.

* **What is an Explicit Intent? **An explicit intent is most commonly used when launching an activity \(from another one\) within the same application. With them the component name is generally specified to which the intent has to be delivered

* **What is the different types of  Broadcasts in Android?  **You can compare a sticky broadcast with a sticky note. Someone posts it and you can read when you pass by/your application starts - regardless of when it was posted. An ordered broadcast is like passing a note - it passes from person/application to person/application. Anywhere in the chain the recipient can elect to cancel the broadcast preventing the rest of the chain from seeing it. A normal broadcast.. well, just sends to everyone that's allowed & registered to listen to it.** **

* **What is DDMS and what can you do with it? **Short for _Dalvik Debug Monitor Service_, DDMS is a [GUI](https://www.webopedia.com/TERM/G/GUI.html) debugging application shipped with the [Android SDK](https://www.webopedia.com/TERM/A/Android_SDK.html) that provides screen capture, log dump and process examination capabilities.

* **What is the support library? Why was it introduced? **The [Support Library](http://developer.android.com/tools/support-library/index.html) is generally used when you want to easily support a wider range of OS versions with less version specific source - with it you can use features introduced in higher version of the OS on older platforms without having to worry and check whether this platform has that feature and do something in case it doesn't.

* **What is a ContentProvider and what is it typically used for? **A ContentProvider manages access to a structured set of data. It encapsulates the data and provide mechanisms for defining data security. ContentProvider is the standard interface that connects data in one process with code running in another process.

* **What is ADB? **ADB**, **Android Debug Bridge, is a command-line utility included with Google's Android SDK

* **What is ANR? How can the ANR be prevented? **ANR is Application not responding. to avoid getting it avoid performing work on the UI thread and do it on the background, avoid leak memory from views, activities and close Database connections. check for null to get more safety code \(or move to Kotlin that is much more Null safe then Java\) there are some good libraries that can help you find memory leaks like LeakCanary.
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
* **What is the**`onTrimM`**method?**
* **Is it possible to run an Android app in multiple processes? How?**
* **How does the OutOfMemory happens?**
* **What is a**`spannable`**?**
* **What is renderscript?**
* **What are the differences between Dalvik and ART?**
* **FlatBuffers vs JSON.**
* **What are Annotations**
* **Tell about Constraint Layout**
* **HashMap, ArrayMap and SparseArray**
* **Explain Looper, Handler and HandlerThread. **
* **How to reduce battery usage in an android application? **There are many ways to achieve that, one of them is reduce the REST calls and use local Database to load you data, using the new [Doze](https://developer.android.com/training/monitoring-device-state/doze-standby.html) and removing the amount of SDK's that send information, for example see if you can reduce the amount of Analytics SDK's in your app.
* **What is**`SnapHelper`**? **SnapHelper is a helper class that helps in snapping any child view of the RecyclerView

### 



