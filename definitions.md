


## How Python uses Indentation to control Flow   
Python implements control flow statements, such as if-clauses and for- or while-loops. Python cares about whitespace indentation. In most programming, whitespace indentation - tabs or spaces before each line of code - may be used to make your code more structured and readable, but will in the end be ignored. Not so in Python: Python uses the indentation level to decide which lines of code belong to a control flow statement (also called its block). One of the most distinctive features of Python is its use of indentation to mark blocks of code. Consider the if-statement from this simple password-checking program:   
   

    if pwd == 'apple':   
          print('Logging on ...')    
    else:   
         print('Incorrect password.')    
    print('All done!')     
  

The lines print('Logging on ...') and print('Incorrect password.') are two separate code blocks. These ones happen to be only a single line long, but Python lets you write code blocks consisting of any number of statements.
To indicate a block of code in Python, you must indent each line of the block by the same amount. The two blocks of code in our example if-statement are both indented four spaces, which is a typical amount of indentation for Python.
In most other programming languages, indentation is used only to help make the code look pretty. But in Python, it is required for indicating what block of code a statement belongs to. For instance, the final print('All done!') is not indented, and so is not part of the else-block.

