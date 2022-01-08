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

Avoids coupling the sender of a request to its receiver by giving more than one object to handle the request. Chains the receiving objects and pass the request along the chain until an object handles it.

![Chain of Responsibility Class](/13-chain-of-responsibility-class.svg)

### Command

Encapsulates a request as an object, thereby letting you parametrize clients with different requests, queue or log requests and support undoable operations.

![Command Class](/14-command.svg)

### Interpreter

Given a language, defines a representation for its grammar along with an interpreter that uses the representation to interpret sentences in the language.

(*Dada una representación de una gramática, tenemos una jerarquía de componente que interpretan terminales y no terminales de la gramática. Los componentes se conocen entre sí.*)

### Iterator

Provides a way to access the elements of an aggregate object sequentially without exposing its underlying representation.

(*Una interfaz llamada Iterable que permite crear un Iterator. Cada colección implementa la interfaz Iterable consruyendo el iterador como corresponda. El iterador abstrae el recorrido de una colección con hasNext y next.*)

### Mediator

Defines an object that encapsulates how a set of objects interact. It promotes loose coupling by keeping objects from referring to each other explicitly, and it lets you vary their interaction independently.

(*Tenemos una jerarquía de collegues. En luagr de comunicarse entre ellos lo hacen a través de una clase mediadora.*)

### Memento

Without violaing encapsulation, capture and externalize an object's internal state so that the object can be restored to this state later.

(*El Originator puede crear un objeto Memento con su estado actual y restaurar su estado a partir de un Memento. Otro componente llamado Caretaker es el responsable de almacenar los objetos Memento pero nunca inspecciona su estado intero.*)

### Observer

Defines a one-to-many dependency between objects so that when one object changes state, all its dependents are notified and updated automatically.

(*Tiene un componente Subject (también llamado Observable) al cual se le pueden adjuntar componentes Observer. Cuando se ejecuta notify() en un Observable, se notifica a todos los observadores automáticamente con un callback.*)

### State

Allows an object to alter its behaviour when its internal state changes. The object will appear to change its class.

(*El componente Context define la interfaz para los clientes y contiene un objeto State. Si el estado cambia, cambiará el comportamiento de Context.*)

### Strategy

Defines a family of algorithms, encapsulates each one and makes them interchangeable. It lets the algorithm vary independently from clients that use it.

(*Define una jerarquía de componentes Strategy con una interfaz común y un contexto que utiliza esa interfaz para ejecutar la estratégia o algoritmo.*)

### Template Method

Defines a skeleton of an algorithm in an operation, deferring some steps to subclasses. It lets subclasses redefine certain portions of an algorithm without changing its general structure.

(*El algoritmo abstracto define un templateMethod y varias operaciones primiivas que serán redefinidas en las subclases.*)

### Visitor

Represents an operation to be performed on the elements of an object structure. It lets you define a new operation without changing the classes of the elements on which it operates.

(*Estructura compuesta por varios elementos: ElementA, ElementB, etc. Componente Visitor que tiene los métodos visitElementA, visitElementB, etc.*)
