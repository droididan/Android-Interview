# Design Patterns

This article will cover some main Design Patterns that are relevant to the Android world, all the example are written in awesome `Kotlin` language. Instead of leaving tons of confusing comments in your code, a much better approach is to adopt common design patterns. Design patterns are reusable solutions to common software problems, the patterns will fall into the following categories:

* **Behavioral Patterns** - born to identify common communication patterns between objects and realize these patterns. By doing so, these patterns increase flexibillity in carrying out this communication.
* **Creational Patterns** - design patterns that deal with object creation mechanisms, trying to create objects in a manner suitable to the situation
* **Structural Patterns** - structural design patterns are design patterns that ease the design by identifying a simple way to realize relationships between entities. 

# Behavioral

### Observer Pattern

The observer pattern is used to allow an object to publish changes to its state. Other objects subscribe to be immediately notified of any changes. RxJava/Android is doing a great job by using the observer patterns to observe object or views. \(check this [acrticle](https://github.com/idanbar134/into_the_rx) for more information\)

**Example**

```kotlin
interface TodoChangedListener {
    fun onTodoChanged(todoString: String)
}

class TodoTextChangedListener : TextChangedListener {
    override fun onTodoChanged(todoString: String) = repository.addNewTodo(todoString)
}

// the object to create
class TodoView {

    var listener: TodoChangedListener? = null

    var text: String by Delegates.observable("") { prop, old, new -> 
        listener?.onTodoChanged(new)
    }
}
```

**How Usage**

```
val textView = TextView()
textView.listener = TodoTextChangedListener()
textView.text = "Go to the market"
textView.text = "Do homework"
```

**Result**

```
Text is changed: Go to the market
Text is changed: Do homework
```

### Command Pattern

When you go to a restaurant and you order a nice steak, you don't necessarily know which cook will prepare you beloved meet. you just tell the waiter "Give me meet! now..!" and the scared waiter posts the order in the kitchen for the next available cook. Just like the `Command` Pattern  give you issue requests without knowing the receiver. you encapsulate a request as an object and send it off. who is listening in the other end is a complete different story. for example lets create a Bus with Rx:

**Example**

```kotlin
object RxBus {
    private var bus : Subject<Any, Any> = SerializedSubject<>(PublishSubject.create())
    
    fun getEvent : Observable<Any> = bus
    
    fun post(obj: Any) { bus.onNext(obj)
}
```

This is a simple powerful class that let you take advantage of the RxAndroid library and post object just like you would do with Greenrobot's `EventBus`

**How Usage**

create an object to represent the post

```kotlin
class MyEvent { }
```

On the posting side use the post method like so:

```kotlin
RxBus.post(MyEvent())
```

and on the receiving side listen like so:

```kotlin
RxBus.filter(event -> event is MyEvent)
        .map(event -> event as MyEvent)
        // do some any thing you want
        .subscribeOn(Schedulers.io())
        .observeOn(AndroidSchedulers.mainThread())
        .subscribe()
```

**Result**

# Creational Patterns

### Factory Method Pattern

Instead of constructors, we can use abstraction of the object generation so that type of the object instantiated can be determined at run time

**Example**

```kotlin
interface Dialog {
    val title: String
    fun show()

    // can be extended with more interfaces like: action OK/Cancel
}

class NetworkDialog(override val title: String = "Network Dialog") : Dialog
class ErrorDialog(override val title: String = "Error Dialog") : Dialog

enum class DialogTypes {
    NetworkDialog, ErrorDialog
}

class DialogFactory {
    fun what(type : DialogTypes) : Dialog {
        when(type) {
            NetworkDialog -> return NetworkDialog()
            ErrorDialog -> return ErrorDialog()
        }
    }
}
```

**How Usage**

```kotlin
val networkDialog = DialogFactory().what(DialogTypes.NetworkDialog)
networkDialog.show()

val errorDialog = DialogFactory().what(DialogTypes.ErrorDialog)
errorDialog.show()
```

**Result**

```
show the ErrorDialog...
show the NetworkDialog...
```

### Dependency Injection

**Example**

**How Usage**

**Result**

# Structural Pattern

### Adapter

The adapter pattern converts the interface of a class into another interface the clients expects. This pattern mainly adapts one object to another one. Adapter lets classes work together that couldn’t otherwise because of incompatible interfaces.

**Example**

```kotlin
interface Target {
    fun request()
}

class Adaptee {
    fun networkRequest() {
        api.getUsers()
    }
}

class AdapterClass : Target {

    var adaptee by lazy { Adaptee() }

    override fun request() {
         adaptee.networkRequest()   // POST 
    }
}
```

**How Usage**

```
var target : Target = AdapterClass()
target.networkRequest()
```

**Result**

