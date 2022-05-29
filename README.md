 * Difference between function and constructor
 * difference between property & field
 * Variables
 * Datatype
 * Method  
 *  Main Method & it's arguments
 * Destructor
 * Abstraction
 * Polymorphism
 * Inheritance
 * Encapsulation
 * Interface
 * Collections
 * Structure
 * Enum
 * File Handling
 * Generic 
 * Generic Method
 * Generic Classes
 * Delegates 
 * Serialization
 * comments 
 * var
 * constant
 * operator
 * Operator Precedence
 * compound assignment operators 
 * increment operator
 * if statement
 * switch statement
 * while loop
 * Parameters 
 * Optional Argument
 * Named Argument
 * Passing Argument Types  |  (by ref, by value, by out)
 * Method Overloading
 * Operator Overloading
 * Recursive Method
 * Class  & Object
 * Value & reference types
 * ACCESS MODIFIER
 * Properties
 * Arrays
 * Jagged Array 
 * Static keyword
 * _CONSTANT
 * _static Constructor
 *_static class
 * this keyword
 * readonly modifier
 * INDEXER
 * Exception
 * sealed
 * Namespaces
 * datatype
 * chain constructor
 * Collections
 * List<T>
 * Stack<T>
 * Queue<T>
 * Dictionary<U, V>
 * HashSet<T>
 * CONCEPT LINE
 * extension methods
---------------------------------------------
generics
lambda expression
events & delegates
lambda expression
LINQ
Nullable types
Dynammic
Exception Handling
Async Await
structures
linq


Variables : 
-Programs use data to perform operation
-creating variable reserves memory location or  space in memory for storing value it is called variable because value inside can be changed when program is running
-variable declaration requires data and datatype 
-it is called identifier as it contains letters, number, underscore


 * Datatype : 
-its an attribute that tells the compiler how the data would be used during operation
-every variable (when allocated memory) is stored with certain kind of information like whats the needed memory for variable and what operations can be performed with variable (e.g integer, String.. )
 - char=''
 - string = ""

	//-------------------------------------------------------------------//

Main Method & it's arguments : (static void Main(args[] string){}   )
array of string is passed in  Main method that represent the command-line arguments (which are mostly used when we need to pass information at program runtime for example when we r writing a program that copies files from one to other location than we probably need to give 2 location  to pass them as command line argument) we can omit these argument we are not using them .  (i have tested the CL argumentS by passing them through console and running .exe of the program and iterating the args argument using loop).

	//-------------------------------------------------------------------//

Difference between function and constructor :
  - constructor is special type of function inside class to initialize class member variables at time of  object creation
  - contsructor is speical member of class with no returnType, thats executed at the time of object creation
  - contsructor  is PUBLIC, (e.g this can be used in multiple condition lets say when creating a BankAccount type class you can send email notification to the user but with CONSTRUCTOR you can automatically send email)
  - DEFAULT CONSTRUCTOR has no parameter
  - we paass paramter to the constructor inorder to become able to initialize value at the time of object creation.
  - contructor can be overloaded by using number of variables.

  1 - we can give any suitable name to function but constructor name will be same as class name
  2 - function have returnType but constructor don't have returnType even DON'T void
  3 - constructor are called only at the time of object creation of class but function can be called as much time as you want.
	
Destructor :
as constructor are used at the time of object creation. destructor is automatically invoked at the time object deletion/destruction. destructor can not be called they are automatically invoked. 
_their name is same as the name of class with tilde(~)
_a class can have only one destructor
_ [     ~DogClass(){ //code }        ]
_they are helpful in closing programs, releasing memory and so on.

	//-------------------------------------------------------------------//

 * OOPs is a paradign based on the concept of Objects,  used to promote the reusability of code and to reduce complexity of code

Inheritance :
acquiring the properties of one class into another class. it provides re-usability by allowing us to extend one class into another class
helps us to define a class based on another class.class who inherit the properties are BASE CLASS, the one who inherits the properties are DERIVED CLASS.
 _SingleInheritance : 
	in which there is one base class & one derive class
 _Hierarchical Inheritance :
	multiple derive classes inherits from single base class
 _MultilevelInheritance :
	in which one class is inherited from other derive class
 _hybridInheitance :
	in which one class is inherited into multiple derive classes

=>Inheritance is the way derived class makes use of the functionality of base class & polymorphism is the way base class makes use of implementation of the derived class.

Polymorphism :  
_THERE ARE 2 TYPES OF POLYMORPHISM
RUN_TIME_POLYMORHPISM : overriding a baseclass method (by using Virtual Method) in derive class (by using OverRide) this behaviour can be achieved by METHOD_OVERRIDING
COMPILER_TIME_POLYMORPHISM : defining multiple methods with same name but different number of parameter.it can be achieved by METHOD OVERLOADING
means that a call to a member method will cause a different implementation to be executed  depending upon the type of the object that invokes the method.
_it means that single method can have different implementation.
_one method with different implementation.
_consider a program which allow users to draw different shapes. each shape is drawn differently & you don't know the which shape user will choose. here at this point Polymorphism can be used to invoke proper Draw method of the derived class by Overriding the same method of  base class. 
_base class method use VIRTUAL keyword  which enable us to work with group of related objects in a uniform way. however the derived classes will use the OVERRIDE keyword 
_simply its a way to call a same method with different object causing it to execute differently.
_(a man whos husband , son will responds depends upon who calls like wife or mother depends upon object type)
_Polymorphism can be useful in many cases. For example, we could create a game where we would have different Player types with each Player having a separate behavior for the Attack method.  In this case, Attack would be a virtual method of the base class Player and each derived class would override it.
_polymorphism is used when you have derive classes with same method witth different implementation in each class this behaviour is achieved through virtual method that are overrided in derive classes.

=> Public virtual void myFunctionName(){}
=> Public override void MyFunctionName(){}


Encapsulation :
_is an idea of sourrounding an entity not just to keep whats inside, but also to protect it.
_In Programming, it means combining members together in a class & restricting their access to the inner working of that class ACCESS MODIFIER are used to serve that purpose of defining scope & visibility of a class member.its also called INFORMATION HIDING. 
_data integrity.
_control the way data is accessed & modified. (e.g if one field is declared private in class it cant be accessd directly but by public class member)
_code is easy to access & easy to modify.
_change one part without effectig the other module.

Abstraction :
is a principle of OOP thats used to hide detail & show only essential features of object. abstraction is a process, its an act of hding the relevant qualities and behaviour,  an object should possess however encapsulation is  the actual mechanism by which qualities & behaviour or by which abstraction is implemented.
_abstraction: hide internal detail and showing only the functionality
_abstraction solves the problem at the design level
_encapsulation solves the problem at implementation level
_abstraction is focued on object instead of how it does it 
_encapsulation is related to the internal details  instead of outter details
_ (i interact with phone there are various censors, volumn button, touch space for my interaction which is abstraction meanwhile i am not concerned with anything thats used to implement this touch interface, the circuits or anything which is encapsulation.  think thats how encapsulation is used to implemente abstraction :D)
_abstract method are only permitted in abstract class
_In case of polymorphism, we have different derive classes with same method  having different implementations this behaviour is achieved through virtual methods that are overridden in derive classes so in this case there is no need of virtual method so they are defined using abstract keyword however derive must be defined using override keyword.
_an abstract class also contains non-abstract members
_Abstract method acts like a template for it derive classes means it set some rules what derive class must implement when inheirt abstract class
_Abstract method is implemented with the purpose of being a super class
_abtract class can not be instantiated
_a non-abstract class derived from abstract class must contain the actual implementation of all inherited methods & accessors
_we cannot use 'SEALED' modifier with abstract class as it (seal) prevents class from being inherited  but abstract class requires inheritance
	//-------------------------------------------------------------------//

Interface : 
Interface is a complete abstract class that only contains the abstract member by default so there is no need to write abstract keyword with it. this class is declared using Interface keyword
_its secure form of communication between  objects as we can tell objects that they can safetly access certian methods and properties
_Also all members are always Public so no access modifier can be applied
_Interface can contain properties, methods etc but can not contains FIELDs
_override keyword is also not needed 
_Interface only contains the declaration of the methods, properties and events but no the implementation its left to the class whos implementing the interface
_sometime we PREFER interface over abstract class because in C# we can inherit from one class but we can Implement Multiple Interfaces means we can include behaviours from multiple sources (sort of multiple inheritance) its written like that (       Interface IAnimal      ) (   class className: IShape, IAnimal, IPti   )
_they only contain declration because its inherited by classes & struct

Collections  :
_dynamic array
is a group of object ( whose common classes are list, ArrayList, Hashtable, stack, queue etc) collection types are used to store, manage and manipulate the similar data more efficiently however data manipulation includes CRUD on data in collection there are 2 types of collection 
_Collection classes are specialized classes for data storage and retrieval
_system.collections.generic works on a specific type that's specified in the program don not contain type conversion of overhead, array size is  not fixed, elements can be added or removed at runtime (list, dictionary, sortedlist, stack, queues). Generics allow you to define the specification of the data type of programming elements in a class or a method, until it is actually used in the program. In other words, generics allow you to write a class or method that can work with any data type.

_system.collections works on non-generic can represent data of different type contains type conversion overhead, does not have a fixed size, any number of element can be stored (arraylist, hashtable, sortedlist, stack, queues)
HERE are few operation of collection
-Adding and inserting items to a collection
-Removing and replacing items to a collection
-Finding, sorting, searching items
-Replacing items
-Copy and clone collections and items
-Capacity and Count properties to find the capacity of the collection and number of items in the collection

_it is group of related objects that are dynammic unlike arrays they can accomodate and shrink, they are organized into namespaces, they ahve built in methods, some collections are really task specific e.g. Dictionaries are used to represent connection in social websites, Queues are used in Task Schedulers, HashSets are used in Searching Algorithms


Generics : 
- IT  WAS MADE TO address the issue of type-safety. generics was introduced  in .net framework to create classes, structures, interfaces, methods.
- when we don't know the type of  object we use generics so it allows us to handle objects with unknown datatypes. it helps us in class Implementation when only dataType of classes are different we pass parameters that would be used in class as datatype however their type would be specified by the arguments passed
- Generics allows you to define the specification of datatype in a class or method UNTILL it's actually used in program.
- in other words allows us to write class or method that can work with any datatype (again datatype would be defined by agumrnts passed).
- .NET framework provides an extensive set of interfaces and classes in the System.Collections.Generic namespace for implementing generic collections.


Generic Classes : 
_generic types also used with class
_it is mostly used with collection of item when same process of adding/deleting items is used throughout regardless of the data beng stored 
_in generic class we do not need to define the generic type for its method because the generic type is already define on the class level

 
	//-------------------------------------------------------------------//

Serialization :
_it is the process of converting object into Stream of Bytes to store the object to memory, database or a file its main purpose is to store the state of object inorder to be able to recreate it when needed the reverse process is - deserialisation
_often times we need to store objects/member variable to physical storage/disk file is - serialisation 
_ workflow of serialisation ( Object => Bytes => db,memory,file )
_the process of reading a object from the file where it is stored - deserialisation
 
	//-------------------------------------------------------------------//


Structure : 
_struct type is value type used to encapsulate small group of related items or it helps you to make a single variable hold related data of variuous datatype 
_collection of variables of different datatype under single unit struct is user defined datatype
_struct shares same syntax as classes but they are limited in terms that it does not allow inheritance & can be instantiated without new keyword & cannot contain virtual method
_they contain method, properties/auto-implemented properties, indexer & so on unlike c or c++
_CANNOT have default constructor but can contain contructor with parameter because struct is value which provides default value for initialization
_all standard c# types (int,float,double etc ) are structs
_Struct do not support destructor
_constructor can also be chained inside the struct chain constructor
_when one constructor is chained to another constructor, the constructor being chained to is executed first. one constructor call another to help it initialize the data in the class
_structure object can be created with or without NEW keyword, when we use new keyword parameterless constructor is called which initialize the members to their default value however if we do not use the new keyword no contructor gets called so no value is assigned to memebers which causes an error so we should assign value to members in that case (    ObjectName.MemberName=45;    )
_default modifier is INTERNAL for structure
_struct also allows the nesting of structure
_struct can not contain default constructor only accepts parameterised or static constructorf
_The basic reason of creating struct is to make type with value semantics (value type) which if managed properly can leads to better performance in managed environment (value type store value in STACK which is faster relative to HEAP)
_CLASSES are reference type structs are value type
_CLASSES can not be initialzed without new operator
_CLASSES support inheritance but struct do not
_STRUCTURES do not have default constructor
_CLASSES are generally used to tackle more complex data while structs are used for small data structures thats intended not to be modified after struct is created while CLASS data usually gets modified

 
	//-------------------------------------------------------------------//

Enum : 
_enum is used to declare a list of NAMED integer (int) constants (else we have to cast it) so that constant integer can be referred using this name by default first variable will have 0 as its value incase we do not assign it a value
_enum can NOT be used with string type
_bunch of cOnstant that we associate with name
_ basically enum define variable that represent the members of a fixed set
_It is used to assign names or string values to integral constants
_enum is a value type, its a set of related named constants often referred to as an emumerator list (   enum Day {Sun, Mon, Tue, Wed}     )
_Enum keyword is used for declaration its primitive datatype which is user-defined
_default datatype of enum is INT if anyother is used we have to cast it
_if any variable is not assigned a value then value of previous variable is assigned to it with increment (variable+1)
_enum is enumerated datatype in c#
_enum is strongly typed constant (enum of one type can not be assgined to other type even though their value is same)
_enum can also be used as namespace
_ Enumeration is declared using enum keyword directly inside a namespace, class, or structure.
_Use of enum makes code more readable and manageable.


File Handling :
_Sytem-IO namespace has various classes to work with files (open,read,write,close)
_FIle is a static class to read/write from physical file
_AppendAllText() - appends text to the end of the file.
_Create() - creates a file in the specified location.
_Delete() - deletes the specified file.
_Exists() - determines whether the specified file exists.
_Copy() - copies a file to a new location.
_Move() - moves a specified file to a new location

Generic : 
_generic allow the reuse of code accross different types it can be used with classes, methods & other
_generic ensures type-casting in c#
_the basic limitation of collection is that it accept every type of object which violates c# rule of type-safety as every class extends from base class of c# use of collection cause major performance overhead.
_helps in code reusability
_type-casting
_Generics can be applied to interface, abstrct class, method, static method, property, event, delegate and operator.
_Generics performs faster by not doing boxing & unboxing.

Generic Method :



Delegates :
_delegates in c# are type-safe function pointer that holds the reference to a method then call that method for execution
_its an object that points toward the function or its reference type variable that holds reference to the method
_the signature of delegate should be same as of method
_they can be attached to Event so whenever button clicked tis funciton will be called.
_its a user-defined type so efore invokign a method using delegate don't forget to instantiate & define the delegate
_signature of delegate should be same as that of method
_It is similar to the class so when we create object of it we have to create the object and pass the function name as parameter in constructor so deleg. can point to it
_if deleg point towards single function it UNICAST DELEGATE if multiple function we call it MULTI_CAST DELEGATE
_it can help function to be passed as parameter.
	=? delegate <returnType><delegateName><parameterList>
	=>public delegate int myDelegate(string s);
this delegate can call method which has int as returnType and string as parameter
delegate object should  be called with new operator

=>public delegate int myDelegate(int n);
class yum{
	myFnctio1(int add){return add;}
	myFnctio2(int multiply){return multiply;}
}
myDelegate a=new myDelegate(myFnctio1);
myDelegate  b=new myDelegate (myFnctio2);
or  myDelegate  printDel=myFnctio1;

a(25);
console.write(showResult())
b(33);
	//-------------------------------------------------------------------//

 - comments : are explanatory statement that developer include in the program to benefit the reader of code reader. 

 - var : datatype is used to implicitly initialize the local variable means it tells the compiler to figure out the type of variable at the time of compilation. implicity typed variables must be initialized

 - constant : constant is used to store a value that can not be changed after initial assignment. to declare constant we use CONST modifier.

 - operator : is a symbol thats used to perform mathematical or logical operation.(arthematic includes DMAS, modulus likes)

 - Operator Precedence : it determines how the expression would be evaluated and the grouping of the terms in expression (DMAS)
 
 - compound assignment operators : that perform an operation and an assignment in one statement. (a+=b)

 - increment operator : have 2 types 
	_Prefix :  increments the value then proceed with the expression.
	_Postfic : evaluates the expression than increments the value.

 - The if statement is a conditional statement that executes a block of code when a condition is true.
 - relational operator are used to evaluate the condition. (>=, <=, ==, !=)

-switch statement test the variable for equality
switch(){
case 1: //expression check
break; //break is used to terminate the statements
default: //else case when condition runs
break;
}

	//-------------------------------------------------------------------//

  -  while loop : 
it repeatedly executes a block of code as long as given condition is true
 - loop will continue indefinitly if statement doesnot evaluate to false
while(condition)
{}
  -  for loop :
executes a set of statements a specific number of times
  -  do-while loop : 
runs atleast once.

	//-------------------------------------------------------------------//

 * Method  :  is a group of statement that can perform a certain task
   - re-usability of code 
   - modification of medthod do not effect the overall program
   - method can effect multiple inputs
   - easy to test
 - method declaration includes <returntype> <methodName> <optional parameter>

	//-------------------------------------------------------------------//

 - Parameters : can accept the value that are passed into the method
 - Optional Argument : when defining method you can give default value for optional parameter. ITS Important the optional parameter must be defined after the required parameter. however if the corresponding parameter is missing then method will use the default value
 - Named Argument : frees you from remembering the order of parameter in which they are passed. Named parameter function call is '   Area(w:5, h:6);   '

	//-------------------------------------------------------------------//

  -  Passing Argument Types :
arguments are passed by 3 ways, by value (by default), by reference, by output
- in Pass By Value, we pass value(int, float etc) of arguments into the method's parameters then we can change the parameter without having an effect on the argument.
-in Pass By Reference, copies an argument's memory address into the formal parameter, inside the method the address is used to access the actual argument used in the call. this means that changes made in the formal parameter also effects the argument. REF keyword is used in both call and method definition to for this.
-in Passing By Output, similar to pass by reference except that they are used to pass value out of the method (get value from method rather from function call)rather than accept data in. They are defined using OUT keyword both at function call & function definition.

	//-------------------------------------------------------------------//

Method Overloading : 
is when multiple methods have SAME NAME but different parameters. parameter can be different by datatype, by sequence, by number of parameter. 

Recursive Method : is one that calls itself till non negative number.  in recursion there is a BASECASE whihc acts as a exit statement .  (4! =  4*3*2*1 = 120)

Operator Overloading : 
most operator in c# can be overloaded they can be redefined for the custom action (e.g to sum the 2 objects). 
all  aethematic & comparison operator can be overloaded  for instance we could define greater than or lesser than valur and return the result with boolean. 
_operator overlaoding method have special name OPERATOR+ (or whichever operator you are using)
_Just keep in mind that when overloading the greater than operator, the less than operator should also be defined.

	//-------------------------------------------------------------------//

Class  & Object : 
-Just like datatype is used to store value in a variable 
_in OOP, class is a datatype(DT) that defines a set of variables & methods for declared object (just like built-in DT stores single value in a variable). class is a blueprint, that defines the data and behaviour for the types. 
_Just like house is divided into rooms  and each room is related to a person
_class definition starts with    -     CLASS keyword <ClassName> {}
_class defines DT for the object but its not an object itself.

_OBJECT is concrete entity based on a class sometime called as  ' Instance of Class ' 
_just as built-in DT are used to declare multiple variables similarly classes are used to declare multiple objects (as an analogy we make a blueprint [which is a class]  before making a building similar blueprint can be used to make several other buildings [objects]). this process of making objects is called 'instantiation'.
_each object has its own characteristics called as Properties. value of these prop can define current state of the object (person is 30 year old, name is Ali)
-Just like datatypes are used to declare multiple variable same way class is used to declare Multiple Objects


	//-------------------------------------------------------------------//

 - ACCESS MODIFIER are used to specify the accessbility of fields or methods. they are (public, private, protected, internal, protected internal). members are private by default.
 _public access modifier makes members accessible from outside the class.
_private restricts them to the classs only.
_

	//-------------------------------------------------------------------//

Value & reference types : 
_there are 2 ways of storing data in c#. value type & reference type. 
_value stored in built-in DT are value types storage. they are stored in STACK struct is also a value type but still user can modify it which is why its called user-defined datatype
_it directly stores value rather than memory address.
_value type provides default value for initialization
_all value type (int,bool,char) are struct
_STACK have memory allocation at compile time(when code is getting converted to exe file)

-REFERENCE TYPES : 
_ are used to store the objects  e.g when we make object of class they are stored as reference types.
_reference types are stored in part of memory called as HEAP.
_when we instatiate object its data is stored in the form of HEAP and the memory addrss of heap is stored in the form of STACK.
_when object of class is created the variable to which the object is assigned holds only a reference to that memory however when the object reference is assigned to a new variable that variable still points to that original object
_HEAP have dynammic memory allocation when EXE file is running

	//-------------------------------------------------------------------//

Properties :
is a member that provides special mechanism to encapsulate the data & to read, write&compute the value of private field.
they can be used as if they are public members but they have special methods called accessor that contain executable statement that help in getting or setting the value of the field. 
_VALUE is a special keyword, used to assign a value to the property 
_name of property can be anything but as per Convention it should be same as the name of the PRIVATE FIELD.
_Property is accessed by its name like anyother private member.
_with property we can control the logic of accessing the variable. (e.g. assign age if its > 16)
_AUTO-IMPLEMENTED property are used where we don't want to customise the logic[ e.g. public int Age{get;set} ]

difference between property & field :
_property helps in validating the data 
_property aides when class is extended 
_property supports different accessbility (setter & getter)
_property can show exception but fields can not.
_mostly fields are set as private and property is used to access that field indirectly. (AS PER GOOD PRACTIVE WE SHOULD NOT DECLARE VISIBLE INSTANCE FIELD)
_fields can not be used in interface but property can be used.

	//-------------------------------------------------------------------//

Arrays : 
is data structure thats used to store data. can also say that collection of variable. 
_c# provides number of built-in classes to manipulate data one such class is array.
_since Arrays are object we need to instantiate them with NEW keyword.
(  int[] myArray=new int[5];  )
(  int[] myArray={1, 2, 3};   )
_Arrays in c# are zero based means first element would have index of zero.
_Multi-Dimensional Array is an array with more than one level of dimension.  Its a matrix of Rows & Columns in which minimum 2 for loops are used one for Rows one for Column. its a single block of memory so all of matrix would have same number of column. 
_Curly brackets are used to define value for each row.
_Jagged Array :  is array whose elements are arrays so its basically array of arrays. each element is a single dimensional array so you can access the element in jagged array like this (   e.g. MyJaggedArray[2][4]  ). each array can have different number of column.
_here i am declaring jagged array that contains eight 2-D array
int[][,] myJaggedArray=new int[8][,]
_Length & Rank Properties are used to measure length & diemension of array respectively. it also provides some built-in methods as well.
_String are often think as array but infact we instantiate Object (e.g. this String a = "My Name is Not"  can be accessed by  a[7])
-Array is Reference type.

	//-------------------------------------------------------------------//

Static keyword :
class members (variables, methods, properties)  can be declared  as static, this makes those member belongs to class itself instead of belonging to objects indiviually. becz of their global nature, static members can be accessed directly using classname without object. ( e.g.each time we instantiate class to increase counter of count variable that time counter will increase  remember count is static and its a single copy so whole value of count will increase it will not be different for each object)

_CONSTANT : 
members are static by default. 
[  public const int ConsVariable=0;
   Console.WriteLine( MyClassName.ConsVariable); ] there value can not be changed once assigned

_static Constructor :
it is used to INITIALIZE the static member of class as the class is called anywhere.

_static class :
can not be initialized by object. its useful for containing logical methods & properties. it contains only static members. there are built-in static classes as well (e.g. Math.Pow(), Math.Pi, Math.Sqrt(), Array.Reverse(arr), String.Concat(s1,s2) )
Console is also a static class with .WriteLine() & .ReadKey() like method

Namespaces : 
useful in 2 ways
_namespace declare a scope the contain a specific number of classes/objects that can be built-in or user defined
_namespaces are used to organize the code elements

_we can define our own namespaces aswell
_USING keyword is used to state the given namespace program is using
_.NET framework is used to organize to many classes that can be  built-in or user defined so that it can be easy to handle the application
_declaring namespace helps to group classes & method in larger programming projects *_*
_just like built-in namespace USING SYSTEM which contain Console.Writeline("class & method")
_using System is a global/root namespace 

Exception : 
_abnormal behaviour of program during execution which causes abnormal termination of the system
_it may be due 
 - invalid data input
 - programmer error
 - physical error
Exception Handling : 
_c# provides flexible mechanism to handle except (              try{}catch(exception  e){   //code is here   }               )
_code that is expected to generate error would be placed in try and exception is manual handling incase if error occurs these are some of the common _exception {  FileNotFoundException, FormatException, IndexOutOfRangeException, InvalidOperationException, OutOfMemoryException  }
_Multiple Exception Handling :
tis program handling multiple exceptions
try {
int x=45, y=0;
}
catch (DivideByZeroException e) {
  Console.WriteLine("Cannot divide by 0");
}
catch(Exception e) {
  Console.WriteLine("An error occurred");
}

_FINALLY keyword is -used to write statements that must be executed either exception runs or not (e.g. we are working with files and we want to close files one we run the complete code)* 

 * List<T>
_its similar to array but elements can be remove and added dynmically
_elements are required to be of same datatype

 * Stack<T>
_ Last in First out (LIFO)
_inserting element is pushing and deleting element is popping, Peek() returns top element  (Undo, redo functionalities, parsing expressions (infix to postfix/prefix conversion))

 * Queue<T>
_First in First Out (FIFO)
_inserting element is enqueuing and deleting element is dequeuing
 _scenaio is Printing Document in printer, Calls in call center

 * Dictionary<U, V>
_collection of unique key/value , key is used to access that element, while value is that elements value
_dictionaries are used in database indexing, cache implementation etc
_it require all key/value pair to be of same type


 * HashSet<T>
_set of unique value where duplicates are not allowed
_same datatype
_they are simply set of values
_allow fast searching lookup, removal of item, 
_it allow finding an item by its key (scenario is finding person  by its last name from phone directory)
	//-------------------------------------------------------------------//
this keyword
points towards  the object

 * extension methods
 - Extension methods are additional custom methods which were originally not included with the class.
 - Extension methods can be added to custom, .NET Framework or third party classes, structs or interfaces using namespace.
 - The first parameter of the extension method must be of the type for which the extension method is applicable, preceded by the this keyword.
 - extension method are static methods present in static class

CONCEPT LINE

 - ClassName ObjectName=new ClassName();
here we are making object of  class  type, here we are also instantiating the object using NEW keyword and returning a reference to its location.

 - DOT OPERATOR is used to access the member of the  class.
 - break statement terminate it to the  next line after the  current body.
 - continue statement terminate the current line.
 - both operand must be true iorder to be entire expression to be true incase of AND operator.
 - only one operand is required to be true to make whole expression true incase of OR operator.
 - ALGORITHM :  step-by-step logic of a solution.
 - every C# program has MAIN method because  it an entry point of a program.
 - values stored in built-in DT (int, string) are stored in a location called STACK.
 - STACK is static memory allocation
 - HEAP is dynammic memory allocation which might need extra memory during runtime OBJECT OF Classes are stored in heap DataStructure.
 - FIELDS are variables in C#
 - its good practice in programming to encapsulate member of class and provide access to them only using PUBLIC METHOD
 - For loop iterates through block of statement untill specific expression evaluates to false however foreach treats everything as a collection. for loop can iterate in both direction but foreach can iterate i single forward direction.we can use foreach if the object we want to iterate over implements IENUMERABLE interface hoever need to use FOR if object can only be accessed by index
 - To call a method or any other member from Main directly it should be STATIC as main is static by default
 - this keyword : is used inside class and represents intance/object of that class however its also commonly used to pass the object as parameter ( e.g MyFunctionName(this));
 - readonly modifier :  prevents a class member from being modified it can only be modified through constructor. it different from const  as it can be declared without initialization & readonly can stored value thats result of a calculation.  (e.g  :   private readonly string name="Abd"; )
 - INDEXER : allows object to be indexed like an array. String is an Object of String Class. String Class is an Array of Char Objects. so that's how String implements Indexer. INDEXER is used with collection, array or list.
 - C# DO NOT support multiple inheritance.

 - datatype : is simply an attribute of data which tells compiler how programmer intends to use that data

_public can be accessed from anywhere outside from the class
_private can only be accessed from within class
_protected similar to private but can be accessed from derive class

 - sealed : class can prevent other classes from inheriting it or any of its members. it provides the level of protection so other classes can not inherit it.

_C# supports Nested classes, a class thats member of another class it can also have access modifier. Object can contain other objects like car can have motor both arw object having their own properties.
_Strings are nullable in c#
	




  


	

