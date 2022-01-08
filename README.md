Design Patterns
===============

Design patterns are common solutions to recurring problems in software design that have evolved over time.

Class diagram
-------------

* Box: class name, mehods, fields
* Diamond based arrow: aggregation, part-of relationship
* Simple arrow: acquaintance, has a reference to relationship
* Dashed arrow: creates relationship
* Triangle: inheritance

Creational
----------

### Abstract Factory

Provides an interface for creating families of related objects without specifying their concrete classes.

---

![Abstract Factory Class](/01-abstract-factory-class.svg)

---

### Builder

Separates the construction of a complex object from its representation so that the same construction process can create different representations.

---

![Builder Class](/02-builder-class.svg)

---

![Builder Interaction](/02-builder-interaction.svg)

---

### Factory Method

Defines an interface for creating an object, but let subclasses decide which class to instantiate.

---

![Factory Method Class](/03-factory-method-class.svg)

---

### Prototype

Specifies the kind of objects to create using a prototypical instance, and creates new objects by copying this prototype.

---

![Prototype Class](/04-prototype-class.svg)

---

### Singleton

Ensures a class only has one instance, and provide a global point of access to it.

---

![Singleton Class](/05-singleton-class.svg)

---

Structural
----------

### Adapter

Converts the interface of a class into another interface clients expect. It lets classes work together that couldn't otherwise because incopatible interfaces.

---

![Adapter Class](/06-adapter-class.svg)

---

### Bridge

Decouples an abstraction from its implementation so that the two can vary independently.

---

![Bridge Class](/07-bridge-class.svg)

---

### Composite

Composes objects into tree structures to represent part-whole hierarchies. It lets clients treat individual objects and compositions uniformly.

---

![Composite Class](/08-composite-class.svg)

---

### Decorator

Attaches additional responsibilities to an object dynamically. It provides a flexible alternative to subclassing for extendig functionality.

---

![Decorator Class](/09-decorator-class.svg)

---

### Facade

Provides a unified interface to a set of interfaces in a subsystem. It defines a higher-level interface that makes the subsystem easier to use.

---

![Decorator Class](/10-facade-class.svg)

---

### Flyweight

Uses sharing to support large number of fine-grained objects efficiently. Shares the common parts to reduce the memory usage.

---

![Flyweight Class](/11-flyweight-class.svg)

---

### Proxy

Provides a surrogate or representative for another object to control access to it. It allows you to do something before or after the request reaches the original target.

---

![Proxy Class](/12-proxy-class.svg)

---

Behavioral
----------

### Chain of Responsibility

### Command

### Interpreter

### Iterator

### Mediator

### Memento

### Observer

### State

### Strategy

### Template Method

### Visitor