## Section 1: `__init__`, `__new__`, and Initialization

### Understanding Initialization

When you create a new instance of a class in Python, there are two key methods that control this process:

1. **`__new__`**: This method is responsible for *creating* a new instance of the class. It's called before `__init__` and is actually a static method (though we don't declare it with `@staticmethod`). It receives the class itself as its first argument, followed by any other arguments.

2. **`__init__`**: This method is responsible for *initializing* the instance after it's been created. It receives the instance (self) as its first argument, followed by any other arguments.

The typical workflow is:
1. `__new__` creates and returns a new instance of the class
2. `__init__` initializes that instance with attributes and behavior

Most of the time, you only need to implement `__init__` because Python's default `__new__` does exactly what you want: it creates a new instance of your class. However, there are scenarios where custom `__new__` implementations are valuable:

- Creating singleton classes (where only one instance can exist)
- Implementing factory patterns (where a method decides which type of object to create)
- Modifying instance creation (e.g., to enforce constraints on what can be created)
- Implementing immutable types (where the instance cannot be modified after creation)

**Key Differences:**
- `__new__` creates the object and returns it
- `__init__` initializes the object and returns None (trying to return anything else raises a TypeError)
- `__new__` can return an instance of a different class if needed
- If `__new__` doesn't return an instance of the class, `__init__` is not called

Here's a simple example showing both methods:

```python
class Person:
    def __new__(cls, name, age):
        print(f"Creating a new Person with name={name}, age={age}")
        # Call the parent class's __new__ method to create the instance
        instance = super().__new__(cls)
        return instance
        
    def __init__(self, name, age):
        print(f"Initializing Person with name={name}, age={age}")
        self.name = name
        self.age = age
```