# Design Patterns

Design Patterns are  these patterns are categorized into 3 main groups:

* **Behavioral Patterns** - born to identify common communication patterns between objects and realize these patterns. By doing so, these patterns increase flexibillity in carrying out this communication.
* **Creational Patterns** - design patterns that deal with object creation mechanisms, trying to create objects in a manner suitable to the situation
* **Structural Patterns** - structural design patterns are design patterns that ease the design by identifying a simple way to realize relationships between entities.

# 

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

**Example**

```
val textView = TextView()
textView.listener = TodoTextChangedListener()
textView.text = "Go to the market"
textView.text = "Do homework"
```

**Output**

```
Text is changed: Go to the market
Text is changed: Do homework
```



