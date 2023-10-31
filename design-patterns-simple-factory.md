Anyone who has taken an object-oriented course likely has used this pattern (I learned it in the [Java course on Code With Mosh](https://codewithmosh.com/p/the-ultimate-java-mastery-series)). Regardless, it is a valuable pattern that should be in your toolkit when working with object-oriented code. I will be using Java to demonstrate this design pattern in action.

## What Is It?
A simple factory is an object that instantiates other objects. Simple factories do this by calling a static method that calls the constructor of the resultant object. Simple factories instantiate one or more types of objects. 

In this article, we will be implementing a pencil factory. We can pass arguments such as type and lead thickness to create pencils with the specified properties. We don't have to worry about the implementation details; we pass arguments to the factory, which returns a pencil.

Some may say that the simple factory pattern is not a design pattern but a stepping stone to the abstract factory or factory method design patterns. However, I disagree, as the simple factory pattern is a flexible and reusable unit of code. Regardless of which side of the fence you are on, the simple factory is an excellent addition to your engineering toolkit.

## Why Use It?
Often, creating objects is more complicated than a simple constructor call with no arguments. You may want to create multiple instances of the same class with different constructor arguments. Or, you may want to use logic to determine the type of object to create. A simple factory allows you to encapsulate this creation logic and only worry about passing the correct arguments. You call the simple factory's creation method, pass it the correct arguments, and it returns the proper object.

## Code Explanation
The code in this article can be found [here](https://github.com/jakeEspinosa/designPatterns).
In this example, we will 
There are a few steps to implementing the simple factory design pattern:

1. Create an interface
2. Implement a class (or classes) against the interface
3. Create a factory class
4. Use the factory

### Create an Interface
First, we create an interface for pencil classes to implement. This interface can implement wooden pencils, mechanical pencils, etc.
```
public interface Pencil {  
    public String getType();  
    public float getLeadThickness();  
}
```
### Implement the Interface
Next, we create a class that implements the interface.
```
public class MechanicalPencil implements Pencil {  
    private String type;  
    private float leadThickness;  
  
    public MechanicalPencil(String type, float leadThickness) {  
        this.type = type;  
        this.leadThickness = leadThickness;  
    }  
  
    public String getType() {  
        return this.type;  
    }  
  
    public float getLeadThickness() {  
        return this.leadThickness;  
    }  
  
}
```
### Create a Factory
Next, we create a factory class that will instantiate objects.
```
public class PencilFactory {  
    public static Pencil makePencil(String type, float leadThickness) {  
        return new MechanicalPencil(type, leadThickness);  
    }  
}
```
### Use the Factory
Last, we use the factory to instantiate objects.
```
public class App {  
    public static void main(String[] args) {  
        Pencil mechanicalPencil = PencilFactory.makePencil("mechanical", 0.9f);  
        System.out.println(mechanicalPencil.getLeadThickness());  
        System.out.println(mechanicalPencil.getType());  
    }  
}
```

## Takeaway
Design patterns are helpful solutions to common software engineering problems. The simple factory pattern is useful for encapsulating object creation logic. Design patterns shouldn't be a hammer looking for a nail, but when appropriate, they dramatically increase the reusability and flexibility of object-oriented software.
