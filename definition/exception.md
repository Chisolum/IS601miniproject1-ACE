# Exception

An Exception is an error that occurs during the execution phase of a program. Whenever there is an error, Python generates an exception that could be handled, which help prevents the program from failing. In other words, it generates a general mechanism for adding error-handling logic to programs. 
Furthermore, raising an exception is a technique for interrupting the normal flow of execution in a program. An exception can be handled by an enclosing try statement. A try statement consists of multiple clauses; the first begins with try and the rest begin with except (provided by :
try:
    <try suite>
except <exception class> as <name>:
    <except suite>
...
