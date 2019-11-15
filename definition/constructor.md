# Constructor 

A constructor is a type of function which is used to initialize the instance members of the class.
Constructors can be of two types.
-Parameterized Constructor – constructor with arguments
-Non-parameterized Constructor – constructor that does not manipulate values
Constructor definition is executed when we create the object of this class. Constructors also verify that there are enough resources for the object to perform any start-up task.
In python, the method __init__ creates the constructor of the class (when the class is instantiated). We can pass any number of arguments at the time of creating the class object, depending upon __init__ definition. Lastly, every class must have a constructor, even if it simply relies on the default constructor.


Below is an example of beginning a constructor:

class C:
    def __init__(self):
        print('Constructor name.')

    def see(self):
        print('C')
