# Intermediate_advanced_python_learning
Continuing my journey of python programming, graduating from a terminal intermediate programmer to an advanced one. This is also an experiment in using AI to create paths of self-learning. This was a learning path suggested by Claude Sonnet 3.7 using a general self-assessment of my programming skills, and which areas I would like to learn about or improve in. Each section will have it's own folder, where I will attempt exercises and upload the problems and **my** solutions to them. I want to be explicit here: The AI use is to consolidate resources in specific topics to streamline learning in certain areas, all solutions will be from me and **only** me to track/showcase my efforts to learn this material. If there's an x in the box, that means that I have solved some problem using the concept and have committed my problem/solution to the related section's folder.


# Advanced Python Learning Journey

This repository documents my journey learning advanced Python concepts, design patterns, and programming paradigms. Each section focuses on specific topics with implementations, examples, and practical projects to solidify understanding.

## Learning Progress

### 1. Advanced OOP Concepts

#### Dunder (Magic) Methods
- [ ] `__init__`, `__new__`, and initialization
- [ ] String representation: `__str__`, `__repr__`
- [ ] Comparison methods: `__eq__`, `__lt__`, etc.
- [ ] Container methods: `__getitem__`, `__setitem__`, `__len__`, etc.
- [ ] Callable objects: `__call__`
- [ ] Context management: `__enter__`, `__exit__`
- [ ] Operator overloading: `__add__`, `__mul__`, etc.
- [ ] Attribute access: `__getattr__`, `__setattr__`, `__getattribute__`

**Project:** Custom Collection Class
- Implement a specialized collection class (like a time series, priority queue, or multi-dimensional vector) that uses appropriate dunder methods to behave like a native Python object

#### Properties and Descriptors
- [ ] Property decorator: `@property`, `@setter`, `@deleter`
- [ ] Descriptor protocol
- [ ] Custom descriptors
- [ ] Computed attributes
- [ ] Attribute validation

**Project:** Data Validation Framework
- Create a framework that uses descriptors to validate class attributes (type checking, range validation, regex pattern matching)

#### Method Resolution Order and Multiple Inheritance
- [ ] Python's C3 linearization algorithm
- [ ] Diamond problem and solutions
- [ ] `super()` function and cooperative inheritance
- [ ] Mixin classes and their application
- [ ] Abstract base classes

**Project:** Plugin System
- Design a plugin system using inheritance and mixins where various feature sets can be combined in different ways

### 2. Design Patterns in Python

#### Creational Patterns
- [ ] Factory Method
- [ ] Abstract Factory
- [ ] Builder
- [ ] Singleton
- [ ] Prototype
- [ ] Object Pool

**Project:** Document Generator
- Create a system that can generate different types of documents (HTML, PDF, Markdown) using appropriate creational patterns

#### Structural Patterns
- [ ] Adapter
- [ ] Bridge
- [ ] Composite
- [ ] Decorator
- [ ] Facade
- [ ] Proxy
- [ ] Flyweight

**Project:** GUI Component Library
- Implement a simple GUI component library that uses structural patterns to compose, extend, and manage UI elements

#### Behavioral Patterns
- [ ] Chain of Responsibility
- [ ] Command
- [ ] Interpreter
- [ ] Iterator
- [ ] Mediator
- [ ] Memento
- [ ] Observer
- [ ] State
- [ ] Strategy
- [ ] Template Method
- [ ] Visitor

**Project:** Workflow Engine
- Build a workflow engine that processes tasks through various stages, using appropriate behavioral patterns to handle state transitions, strategies for different processing requirements, and commands for user operations

### 3. Functional Programming in Python

#### First-Class Functions
- [ ] Functions as arguments
- [ ] Functions as return values
- [ ] Closures and scope
- [ ] Partial application
- [ ] Higher-order functions

**Project:** Custom Function Toolkit
- Create a toolkit of higher-order functions for common operations (caching, logging, timing, retry logic)

#### Decorators
- [ ] Function decorators
- [ ] Class decorators
- [ ] Decorator factories with parameters
- [ ] Stacking decorators
- [ ] Functools module (`@wraps`, etc.)

**Project:** API Framework
- Develop a mini web API framework that uses decorators for routing, authentication, rate limiting, and response formatting

#### Functional Utilities
- [ ] `map`, `filter`, `reduce`
- [ ] List/dictionary/set comprehensions
- [ ] Generator expressions
- [ ] Lambda functions
- [ ] Immutability concepts

**Project:** Data Processing Pipeline
- Implement a data processing pipeline that transforms, filters, and aggregates data using functional programming techniques

### 4. Advanced Python Features

#### Metaclasses
- [ ] Understanding Python's type system
- [ ] Creating custom metaclasses
- [ ] Class creation hooks
- [ ] Attribute control with metaclasses
- [ ] Framework construction with metaclasses

**Project:** ORM System
- Build a simple Object-Relational Mapping system that uses metaclasses to transform class definitions into database operations

#### Context Managers
- [ ] `with` statement mechanics
- [ ] Implementing `__enter__` and `__exit__`
- [ ] The `contextlib` module
- [ ] Nested context managers
- [ ] Context managers for resource management

**Project:** Resource Manager
- Create a comprehensive resource management system for handling different types of resources (files, network connections, locks) with proper cleanup

#### Generators and Coroutines
- [ ] Generator functions with `yield`
- [ ] Generator expressions
- [ ] Send/throw/close methods
- [ ] Bidirectional communication
- [ ] Pipeline patterns with generators
- [ ] Simple coroutines

**Project:** Event Processing System
- Develop an asynchronous event processing system using generators to handle event streams

### 5. Advanced Modules and Techniques

#### Concurrency and Parallelism
- [ ] Threading and the Global Interpreter Lock (GIL)
- [ ] Multiprocessing
- [ ] Concurrent.futures module
- [ ] Asyncio basics
- [ ] Locks, queues, and synchronization

**Project:** Web Scraper
- Build a concurrent web scraper that can efficiently download and process multiple web pages

#### Metaprogramming
- [ ] AST module
- [ ] `exec`, `eval`, and their uses
- [ ] Dynamically generating code
- [ ] Introspection and reflection
- [ ] Monkey patching

**Project:** Test Mocking Framework
- Create a framework that can dynamically replace or modify function behavior for testing purposes

#### Performance Optimization
- [ ] Profiling and benchmarking
- [ ] Memory usage optimization
- [ ] Algorithmic optimization
- [ ] Cython integration
- [ ] Numba for numerical computing

**Project:** Performance Analysis Tool
- Build a tool that can analyze and visualize the performance of Python code, suggesting optimization strategies


## Development Process

1. For each topic:
   - Study the concept and its Python implementation
   - Write example code demonstrating the concept
   - Document key insights and gotchas
   - Complete the associated project
   - Mark as complete in this README

2. Commit strategy:
   - Make atomic commits with descriptive messages
   - Reference learning resources in commits when applicable
   - Tag important milestones

## Future Exploration Ideas

- Type hints and static type checking
- Python internals and CPython
- Creating Python packages and publishing
- Domain-specific language implementation
- Creating Python C extensions

