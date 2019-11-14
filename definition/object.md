# Objects
An object is created using the constructor of the class. This object will then be called the instance of the class. Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. You can create multiple different objects that are of the same class (have the same variables and functions defined). However, each object contains independent copies of the variables defined in the class. For instance, if we were to define another object with the "NewClass" class and then change the string in the variable.  :    


>class NewClass:  
>    name = ‘Jane’  
>Newobjectx = NewClass()   
>Newobjecty = NewClass()  

>Newobjecty.variable = "Doe"


To access a function inside of an object you use notation similar to accessing a variable:    

>class NewClass:
>    name = ‘Jane’
>Newobjectx = NewClass()   

>Newobjecty.functions()     





