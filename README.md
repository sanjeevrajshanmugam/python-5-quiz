# python-5-quiz


# What will happen if an object has circular references?

Question 1 Answer
a.

The destructor will be called when the program ends

b.

The destructor (__del__) will not be called automatically
c.

The destructor is immediately called when del obj is executed
d.

It results in a RecursionError

# What will `print("Hello" + "World")` output?
Question 2 Answer
a.
Hello World
b.
Hello + World
c.
HelloWorld
d.
"HelloWorld"
# What will be the output of the following code?

class A:

    def __init__(self):

        print("A's constructor called")

        self.value = 10


class B(A):

    def __init__(self):

        print("B's constructor called")

        self.value = 20


obj = B()

print(obj.value)


Question 3 Answer
a.

A's constructor called

B's constructor called

10


b.

B's constructor called

A's constructor called

10


c.

B's constructor called

20


d.

Error
# What happens if a destructor (__del__) method creates a new reference to the object being deleted?
Question 4 Answer
a.

The object is deleted normally
b.

The object will never be deleted
c.

Python raises an error
d.

The object is deleted but produces a warning
# What happens when you use the `else` block along with `try-except`?
Question 5 Answer
a.
The `else` block is executed only if an exception occurs in the `try` block.
b.
The `else` block is executed only if no exception is raised in the `try` block.
c.
The `else` block is always executed before `finally`.
d.
The `else` block is executed after the `except` block.

# What does `my_list = [1, 2, 3]; my_list.extend([4, 5])` do?
Question 1 Answer
a.
Replaces the list with [4, 5]
b.
Removes elements from the list
c.
Appends [4, 5] as a single element
d.
Adds 4 and 5 as separate elements
# What will `tuple(range(3))` return?
Question 2 Answer
a.
(0, 1, 2)
b.
(1, 2, 3)
c.
Error
d.
(0, 1, 2, 3)
# What will be the output of the following code?

class A:

    def __init__(self):

        print("A's constructor")


class B(A):

    def __init__(self):

        print("B's constructor")

        super().__init__()


obj = B()


Question 3 Answer
a.

B's constructor

A's constructor


b.

A's constructor

B's constructor


c.

No output
d.

Error

# Which method is used to read all the lines from a file as a list in Python?
Question 4 Answer
a.
`read()`
b.
`readlines()`
c.
`readall()`
d.
`readline()`
# What happens when you try to modify a tuple element?
Question 5 Answer
a.
A TypeError occurs
b.
The modification is ignored
c.
The tuple is automatically converted to a list
d.
The element is modified successfully
# What happens if you try to access an index that is out of range?
Question 2 Answer
a.
Returns False
b.
Raises an IndexError
c.
Returns an empty list
d.
Returns None
# What will be the output of this code?
my_dict = {'a': 1, 'b': 2, 'c': 3}
for key in my_dict:
print(key, my_dict[key])
Question 3 Answer
a.
It prints the keys but not the values.
b.
It prints only the values.
c.
It prints the keys and their corresponding values.
d.
It raises an error since my_dict cannot be iterated this way.
# What will be the output of the following code?

class A:

    def __del__(self):

        print("Destructor of A")

 

obj1 = A()

obj2 = obj1

del obj1

print("End of Code")

del obj2

Question 4 Answer
a.

Destructor of A
End of Code

b.

End of Code
Destructor of A
c.

Destructor of A
d.

Error
# What will be the output of the following code?

class A:

    def __new__(cls):

        print("A's __new__ method called")

        return super().__new__(cls)


    def __init__(self):

        print("A's constructor called")


obj = A()


Question 5 Answer
a.

A's constructor called


b.

A's __new__ method called

A's constructor called


c.

No output
d.
Error

# What will be the output of the following code?

class A:

    def __new__(cls):

        print("A: __new__ called")

        return super().__new__(cls)

    def __init__(self):

        print("A: __init__ called")


A()


Question 1 Answer
a.

A: __new__ called

A: __init__ called


b.

A: __init__ called

A: __new__ called


c.

TypeError: object.__new__() takes no parameters
d.

None
# How do you define a method inside a Python class?
Question 3 Answer
a.
`def method(self):`
b.
`define method(self):`
c.
`class method(self):`
d.
`function method(self):`
# What does the `+` quantifier mean in regex?
Question 4 Answer
a.
Matches one or more occurrences of the preceding character
b.
Matches exactly one occurrence
c.
Matches only digits
d.
Matches zero or more occurrences of the preceding character
# If a class `Person` is defined as follows, how do you access the attribute `name` of an object `p`?
class Person:
     def __init__(self, name):
          self.name = name
p = Person("John")
Question 5 Answer
a.
self.name
b.
p.name
c.
Person(self.name)
d.
Person.name
# What will be the output of the following code?

class A:

    x = 10


class B(A):

    pass


class C(A):

    x = 20


class D(B, C):

    pass


print(D.x)


Question 1 Answer
a.

10
b.

20
c.

Error due to multiple inheritance
d.

None
# Which of the following methods will remove the key 'x' from a dictionary my_dict safely, without causing an error if the key doesn't exist?
Question 2 Answer
a.
my_dict.pop('x', None)
b.
my_dict.pop('x')
c.
my_dict.remove('x')
d.
del my_dict['x']
# Which method is used to initialize objects in Python?
Question 3 Answer
a.
`__create__`
b.
`__init__`
c.
`__start__`
d.
`__new__`
# Which of the following exceptions is raised when you try to access an undefined variable in Python?
Question 4 Answer
a.
IndexError
b.
NameError
c.
KeyError
d.
TypeError
