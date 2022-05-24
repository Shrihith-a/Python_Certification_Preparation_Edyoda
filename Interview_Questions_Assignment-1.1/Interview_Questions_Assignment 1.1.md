# Interview Questions Assignment 1.1
# Find and read 20 interview questions for Data Types, Operators, Conditional Statements, Looping Statements, Functions.

1. What is Python?

        Python is a programming language with objects, modules, threads, exceptions, and automatic memory management. Python is designed to be highly readable. It uses English keywords frequently whereas other languages use punctuation, and it has fewer syntactical constructions than other languages.

2. How is memory managed in Python?

        - Memory in Python is managed by Python private heap space. All Python objects and data structures are located in a private heap. This private heap is taken care of by Python Interpreter itself, and a programmer doesn’t have access to this private heap.
        - Python memory manager takes care of the allocation of Python private heap space.
        - Memory for Python private heap space is made available by Python’s in-built garbage collector, which recycles and frees up all the unused memory.

3.  What is pep 8?

        PEP stands for Python Enhancement Proposal. It is a set of rules that specify how to format Python code for maximum readability.

4. What are docstrings in Python?

        - Docstrings are not actually comments, but, they are documentation strings. These docstrings are within triple quotes. They are not assigned to any variable and therefore, at times, serve the purpose of comments as well.

        """ 
        This is Docstring example
        It is useful for documentation purposes
        """
5. What is a function in Python?

        - A function is a block of code that is executed only when it is called. To define a Python function, the def keyword is used. If the function returning something, they need a return keyword.

                - def example(a):
                        return a*2
6. . What are local variables and global variables in Python?

        - Global Variables:
                Variables declared outside a function or in global space are called global variables. These variables can be accessed by any function in the program.

        - Local Variables:
                Any variable declared inside a function is known as a local variable. This variable is present in the local space and not in the global space.

        - Example of Global Variable
                a = 1
        - Example of Local Variable
                def sample():
                        #Local Variable
                        a = 1

7. What is a lambda function?

        - An anonymous or unnamed function is known as a lambda function. This function can have any number of parameters but, can have just one statement. It is often used as a one-time function rather than a function that used repeatedly.

        # Example of Lambda Function
                test = lambda x,y: x*y
                print(test(2,4))

8. Why lambda forms in python does not have statements?

        A lambda form in python does not have statements as it is used to make new function object and then return them at runtime.

9. What are the supported data types in Python?

        - Python has five standard data types −

                1. Numbers (Integer and Float)
                2. String
                3. List
                4. Tuple
                5. Dictionary

10. What are indexes?

        - To access an element from ordered sequences, we simply use the index of the element, which is the position number of that particular element. The index usually starts from 0, i.e., the first element has index 0, the second has 1, and so on.

        - Example usage of index
                list_ex = [1,2, 'Test']
                print(list_ex[0])

11. What are negative indexes and why are they used?

        - When we use the index to access elements from the end of a list, it’s called reverse indexing. In reverse indexing, the indexing of elements starts from the last element with the index number −1. The second last element has index ‘−2’, and so on. These indexes used in reverse indexing are called negative indexes.

        - Example usage of index
                list_ex = [1,2, 'Test']
                print(list_ex[-1])

12. What is a dictionary in Python?

        - Python dictionary is one of the supported data types in Python. It is an unordered collection of elements. The elements in dictionaries are stored as key-value pairs. Dictionaries are indexed by keys. The data type is presented by{} .

        - Example of Dictionary
                dictionary = {'key' : 'value'}
13. What are lists and tuples? What is the key difference between the two? 
        Solution:
                - Lists and Tuples are both sequence data types that can store a collection of objects in Python. 
                - The objects stored in both sequences can have different data types. 
                - Lists are represented with square brackets ['sara', 6, 0.19], while tuples are represented with parantheses ('ansh', 5, 0.97).
                - The key difference between the two is that while lists are mutable, tuples on the other hand are immutable objects. 
                - This means that lists can be modified, appended or sliced on the go but tuples remain constant and cannot be modified in any manner.

14. What are the common built-in data types in Python?
        Solution:
                There are several built-in data types in Python. Although, Python doesn't require data types to be defined explicitly during variable declarations type errors are likely to occur if the knowledge of data types and their compatibility with each other are neglected. Python provides type() and isinstance() functions to check the type of these variables. These data types can be grouped into the following categories-

                1. None Type: Represents the NULL values in Python.
                2. Numeric Type:
                        1. int: Stores integer literals including hex, octal and binary numbers as integers
                        2. float: Stores literals containing decimal values and/or exponent signs as floating-point numbers
                        3. complex: Stores complex numbers in the form (A + Bj) and has attributes: real and imag
                        4. bools: Stores boolean value (True or False).
                3. sequence Types:
                        1. list: Mutable sequence used to store collection of items.
                        2. tuple: Immutable sequence used to store collection of items.
                        3. range: Represents an immutable sequence of numbers generated during execution.
                        4. str: Immutable sequence of Unicode code points to store textual data.
                4. Mapping Types
                        1. dict: Stores comma-separated list of key: value pairs
                
                5. Set Types:
                        1. set: Mutable unordered collection of distinct hashable objects.
                        2. frozenset: Immutable collection of distinct hashable objects.
                6. Modules:
                        Module is an additional built-in type supported by the Python Interpreter. It supports one special operation, i.e., attribute access: mymod.myobj, where mymod is a module and myobj references a name defined in m's symbol table. The module's symbol table resides in a very special attribute of the module __dict__, but direct assignment to this module is neither possible nor recommended.
    
                7. Callable Types:
                        Callable types are the types to which function call can be applied. They can be user-defined functions, instance methods, generator functions, and some other built-in functions, methods and classes.
                        Refer to the documentation at docs.python.org for a detailed view of the callable types.

15. In Python what are iterators?

        - In Python, iterators are used to iterate a group of elements, containers like the list or string. By iteration, it means that it could be looped by using a statement.
    
16. How can the ternary operators be used in python?

        - The Ternary operator is the operator that is used to show the conditional statements. This consists of true or false values with a statement that has to be evaluated for it.

        - #Ternary operators example
                a = 1 #The true values
                if a < 1:
                        print('Less')
                #If the previous condition haven't fulfilled
                else:
                        print('More')


17. What is a enumerate function in python?

The enumerate() method adds a counter to an iterable and returns it in a form of enumerate object. The object would consist of the counter and the iterable values.

#Enumerate exampleiter_example = ['test', 'test2', 'test3']
for idx, val in enumerate(iter_example):
   print(idx)
   print(val

18. What is Dict and List comprehensions are?

        - They are syntax constructions to ease the creation of a Dictionary or List based on existing iterable. 
        - It is created by looping inside the Dictionary or List object.

        #Dictionary comprehension
                dict_comprehension = {key:val for key, val in emumerate('sample')}
                print(dict_comprehension)#List comprehensionlist_comprehension = [i for i in range(5)]
                print(list_comprehension)

19. What is a shallow copy?

        - Shallow copy is used when a new instance type gets created and it keeps the values that are copied in the new instance. 
        - Shallow copy is used to copy the reference pointers just like it copies the values. 
        - It means when we copying an object to another variable, it would be connected.

        #Example of shallow copy
                list_example = [1,2,3,4,5]
                another_list = list_example
                another_list[0] = 100
                print(list_example)

20. What is a deep copy?

        - Deep copy is used to store the values that are already copied.
        - The deep copy doesn’t copy the reference pointers to the objects. 
        - It makes the reference to an object and the new object that is pointed by some other object gets stored. 
        - Contrast with a shallow copy, The changes made in the original copy won’t affect any other copy that uses the object. It means they are not connected.

        #Example of Deep copy
                list_example = [1,2,3,4,5]#Iniating Deep copy with .copy attribute
                another_list = list_example.copy()
                another_list[0] = 100
                print(list_example)