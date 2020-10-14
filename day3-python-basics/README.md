I compile the content of TryHackCIT with external note resources here.

# Python uses
Python is a general purpose programming language used many domains, like
- web development
- software development
- mathematics
- system scripting

![Image of Python](https://upload.wikimedia.org/wikipedia/commons/f/f8/Python_logo_and_wordmark.svg)


# Python properties
Known for being easy to start learning programming, check out its general properties:
- interpreted programming language 
  - read->execute
  - compiled programming language: read->compile->execute
- object oriented
  - time saving programming paradigm
- cross-platform compatibility
  - runs on Windows, Linux, Mac
- versions
  - Python 2 (deprecated)
  - Python 3

# Python for hacking?
Use Python to automate the boring stuff! Programming is like having a super power, we instruct the computer what to do.
- performing tasks many times
  - brute force logging attempts
  - cracking
  - fuzzing
- automate processes
  - website scraping
 - vast libraries ready to use
   - spoofing MAC address
   - spoofing DNS 
 - packet crafting - scapy
   - wifi deauth attack
   - network scanning
   - network analysis
   
 # Python programs
- file extension for python: .py
- common editors/IDE
  - ![Image of sublime text](https://img.icons8.com/color/48/000000/sublime-text.png)
![Image of vscode](https://img.icons8.com/fluent/48/000000/visual-studio-code-2019.png)
![Image of pycharm](https://img.icons8.com/color/48/000000/pycharm.png)
  
- running python program
  - python file-name.py
 
 ## Installing python
 [Download Python here!](https://www.python.org/downloads/)
 
 ## Hello world!
```python
print("Hello world!")
```

# Python syntax
## Indentation
Indentation indicates a block of code. It must be consistent throughout the end of the source code.

## Comments
Use comments to keep track with what we have written with "#".
### Single line comment 
```python
# This line of code is to assign abc into x
x = "abc"
```
### Multiple line comment
Wrap everything inside 3 double quotes.
```python
"""
# This line of code is to assign abc into x
x = "abc"
"""
```

## Variables
We can assign values into variables.
- Variable names must start with alphabets or underscore
- Use names other than Python keywords (`and, if, else`)
```python
x = "abc"
y = 123
```

# Data types
You don't need to declare data types for variables in Python, and you can change it later.
- string: `"apple"`
- integer: `1`
- boolean: `True`
- float: `1.0`
- list: `["apple", "bear"]`
  - may contain duplicate element
  - elements maintain their order
  - counted from 0
- tuple: `("apple", "bear")`
- dict: `{"fruit": "apple"}`
  - key-value pairs
 
 # Operators
 ## Assignment operators
- equals: `==`
- not equals: `!=`

 ## Arithmetic operators
- addition: `+`
- subtraction: `-`
- multiplication: `*`
- division: `/`

## Logical operators
- `and, or, not`
  
# Python conditions & if statements  
```python
if(condition):
  #trigger this statement
elif(condition):
  #trigger this statement if the above is false 
else:
  #trigger this statement if everything else if false
 ```
 
# Looping
Looping is useful to iterate each element in a list instead of repetitively typing conditions for each element.
 ## for loop
For loops compares elements if the conditition is met.
 ```python
foods = ["apple", "banana", "chicken"]
for food in foods:
  print(food)
  
for index in range(10):
  print(index)
 ```
 
## while loop
While loop compares elements until the condition is no longer met, with 3 components (initialization, condition, increment). 
```python
index = 1
while index < 10:
  print(index)
```
 
# Functions
A function is a block of code that only runs when it is called, this allows reusability of codes.
- You may or may not pass any parameters into a function
- You may or may not have return data
```python
def greeting():
  print("Hello there")

def greeting(abc):
  print("Hello there")  

def greeting(number):
  return number + 1
```
 
