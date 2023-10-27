Programming is both an art and a science. While creativity is essential, established standards and general patterns make writing code easier. Design patterns are templates for object-oriented code that allow you to spend mental energy on functionality rather than implementation. You do not need to memorize them all, but familiarity with the [23 standard design patterns](https://en.wikipedia.org/wiki/Design_Patterns) will serve you well.

## What Are Design Patterns?
According to Wikipedia:

> general, reusable solution to a commonly occurring problem within a given context in software design

Design patterns give you proven solutions to common problems. However, be wary of viewing every engineering problem through the lens of design patterns. They are **solutions to problems**, not something you shoehorn into every codebase. With familiarity and time, you will naturally see problems best solved with a design pattern.

### Creational
Creational design patterns let you abstract away the creation of an object. They are helpful when object creation relies on complex logic or many parameters/attributes.

### Behavioral
Behavioral design patterns deal with algorithms -- behavior -- and let you abstract them away.

### Structural
Structural design patterns concern defining relationships between classes and objects. The relationships allow composing smaller classes and objects into bigger ones.

## Why Use Them?
The purpose of design patterns is two-fold: to make your code more reusable and to save mental energy for other aspects of writing code.

### Reusability
At the heart of every design pattern is reusability and extensibility. They are strategies to flexibly accomplish tasks that can be modified in a logical and consistent way. For example, the [Abstract Factory](https://en.wikipedia.org/wiki/Abstract_factory_pattern) can easily be extended by adding one more class that implements the factory interface. The [Strategy Pattern](https://www.freecodecamp.org/news/a-beginners-guide-to-the-strategy-design-pattern/) can be extended by adding more algorithms that implement the strategy interface. Often, extending code that uses a design pattern is as simple as adding another implementation of an interface.

### Don't Reinvent The Wheel
Design patterns are just that - patterns. They are templates that we can follow to accomplish tasks. Following a pattern saves us the mental energy of devising a maintainable and usable solution and allows us to spend energy on using the solution to solve problems. 

## Resources to Learn Design Patterns
- [Design Patterns: Elements of Reusable Object-Oriented Software](https://www.amazon.com/Design-Patterns-Elements-Reusable-Object-Oriented/dp/0201633612) - book
- [Design Patterns for Humans](https://github.com/kamranahmedse/design-patterns-for-humans) - GitHub

## Takeaway
Design patterns provide proven methods to solve common problems faced in software engineering. They promote maintainable and reusable object-oriented codebases. However, be wary of trying to solve every problem with a design pattern. They are tools, and you should pick the right tool for the job.
