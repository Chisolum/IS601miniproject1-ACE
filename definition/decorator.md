# Decorator
 
A decorator takes a function, extends it and returns, allowing you to make simple modifications to callable objects like functions, methods, or classes.
From the provided example below (https://pythonbasics.org/)  hello() is a decorator.

def hello(func):                                                                                            
    def inner():                                                                                            
        print("Hello ")                                                                                     
        func()                                                                                              
    return inner                                                                                            
                                                                                                            
def name():                                                                                                 
    print("Alice")                                                                                          
                                                                                                            
                                                                                                            
obj = hello(name)                                                                                           
obj()          