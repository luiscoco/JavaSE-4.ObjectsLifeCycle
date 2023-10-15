# JavaSE-4.Objects_LifeCycle

 In Java, the lifecycle of an object refers to its creation, usage, and eventual destruction by the garbage collector. Let me walk you through the different stages with some examples:

Creation (Instantiation):

Objects are created using the new keyword or through a factory method.
Constructors are called during this stage.
java
Copy code
// Example: Creating an object of class Car
Car myCar = new Car("Toyota", "Camry");
Initialization:

After creation, variables are assigned values and other initializations take place.
java
Copy code
// Example: Initializing the car's mileage
myCar.setMileage(10000);
Usage:

The object is actively used to perform operations and tasks.
java
Copy code
// Example: Accelerating the car
myCar.accelerate();
Destruction (Garbage Collection):

When an object is no longer reachable or referenced, it becomes eligible for garbage collection.
The garbage collector automatically identifies and frees up memory occupied by unreferenced objects.
java
Copy code
// Example: Dereferencing the object
myCar = null;
After this point, if there are no other references to the myCar object, it may be garbage collected.

It's important to note that developers don't explicitly destroy objects in Java; the garbage collector takes care of reclaiming memory occupied by objects that are no longer in use.
