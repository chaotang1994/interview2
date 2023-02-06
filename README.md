# interview2






-Describe the newly added features in Java 8?

Lambda Expressions
Functional Interfaces
Stream API
Date and Time API
Interface Default Methods and Static Methods
Method References

-What is Lambda Expression?

Lambda Expression is an anonymous function which accepts a set of input parameters and returns results.
Lambda Expression is a block of code without any name, with or without parameters and with or without results. This block of code is executed on demand


-What are the three parts of a Lambda Expression? What is the type of Lambda Expression?
Can you explain the syntax of Lambda expressions?
Lambda expressions has 3 parts 
part is parameter or argument
arrow operator
statement or lambda expression body

-What is a Functional Interface? What is SAM Interface?
A Functional Interface is an interface, which contains one and only one abstract method. Functional Interface is also known as SAM Interface because it contains only one abstract method.
SAM Interface stands for Single Abstract Method Interface

-Can a functional interface extend/inherit another interface?
A functional interface cannot extend another interface with abstract methods as it will void the rule of one abstract method per functional interface.
It can extend other interfaces which do not have any abstract method and only have the default, static, another class is overridden, and normal methods



-Is it possible to define our own Functional Interface? What is @FunctionalInterface? What are the rules to define a Functional Interface?
Yes, it is possible to define our own Functional Interfaces. We use Java SE 8’s @FunctionalInterface annotation to mark an interface as Functional Interface.
Define an interface with one and only one abstract method.
We cannot define more than one abstract method.
Use @FunctionalInterface annotation in interface definition.
We can define any number of other methods like Default methods, Static methods.

-What is the default method, and why is it required?
A method in the interface that has a predefined body is known as the default method. It uses the keyword default. default methods were introduced in Java 8 to have 
It allows us to provide method’s implementation in Interfaces.
To add new Functionality to Interface without breaking the Classes which implement that Interface.
To provide elegant Backwards Compatibility Feature.
To ease the extension of the existing Functionality.
To ease of Maintain the existing Functionality

-What is method reference in java 8?

Method reference is a shorthand notation of a lambda expression to call a method.
 Method reference to an instance method of an object – object::instanceMethod
 Method reference to an instance method of an arbitrary object of a particular type – Class::instanceMethod
 Method reference to a constructor – Class::new
 Method reference to a static method of a class – Class::staticMethod

-What are some standard Java predefined functional interfaces?
Some of the famous predefined functional interfaces from previous Java versions are Runnable, Comparator, and Comparable.

-What are the various categories of pre-defined function interfaces?
Predicate<T> return boolean,test(), and(), or(),negate().
Consumer<T>accepts a single input argument and returns no result,accept()
Function<T, R>input argument of a certain type and produces a result of another type. apply()
Supplier<T>t takes no arguments and only returns some value.get()
UnaryOperator<T>when the argument and the result are of the same type. Function()


-What are Java 8 streams?
The streams are not collections. streams are WRAPPERS for collections and arrays.They wrap an EXISTING collection (or another data source) to support operations expressed with LAMBDAS, so you specify what you want to do, not how to do it

Streams are immutable
Streams are not reusable
Streams don't store their elements
Streams work perfectly with lambdas

-Why do we require stream API?
It supports Functional-Style programming.
It does faster processing. Hence, it is apt for better performance.
It allows parallel operations.

-What are the main components of a Stream?
A data source
Set of Intermediate Operations to process the data source
Single Terminal Operation that produces the result

-What are Intermediate and Terminal operations?
-intermediate operations:
lazy operator, transforms a stream to another stream,processes the stream data, mostly lambda function, could have one or more intermediate operators.
filter(), map(), distinct(), sorted(), limit()

-Terminal Operations
 always return something other than a stream.
forEach(), toArray(), reduce(), collect(), min(), max(), count(),




