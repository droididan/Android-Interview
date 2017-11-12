# Design Patterns

instead of leaving tons of confusing comments in your code, a much better approach is to adopt common _design patterns. _Design patterns are reusable solutions to common software problems, the patterns will fall into the following categories:

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
showing ErrorDialog...
showing NetworkDialog...
```



### Dependency Injection

**Example**

**How Usage**

**Result**

# Structural Pattern

### Adapter

The _adapter pattern _converts the interface of a class into another interface the clients expects. This pattern mainly adapts one object to another one. Adapter lets classes work together that couldn’t otherwise because of incompatible interfaces.









