Software Carpentry Workshop: Lesson1: Introduction to Python
===


SWC workshop, February 2018  
Instructor: Balan Ramesh  
Time: 3 hours  

---

Good morning!
Before we start working with python, let's make a folder where you will save all your work during this workshop.

Let's make a folder `SWC_spring2018` on your Desktop. We will be working with this folder for the next 2 days so it is better if you leave it on the Desktop where it is easily accesible. It also helps for everyone to have the folder in the same location as it will make it easier to navigate to your files when we start using command line interface later today.

:+1: Do it with students and make sure everyone is with you - put up red sticky notes if having problems, green when done with the task. 

Now let's download datasets (Data.zip) for the workshop and put it in `SWC_spring2018` folder.

[Dataset](https://raw.githubusercontent.com/AnnaWilliford/2017-11-11-UTA/gh-pages/workshop/SWC_fall2017/Data.zip)

When you unzip this file, you should have `Data` folder with `ByCountry` folder and `gapminder.txt` file in it.


Finally, let's make another folder called  `Python_basics` inside `SWC_spring2018` folder. This is where we will save all files for this lesson.

:+1: Do it with students and make sure everyone is with you - put up red sticky notes if having problems, green when done with the task.


Now we are ready to work with Python.

### Learning objectives of this workshop

- Understand benefits of using Python
- Understand how to work with Jupyter Notebook
- Understand how to go get data from Excel to Python
- Understand building blocks of Python language
- Understand how to extract parts of the dataset
- Understand how to write simple Python scripts

Ultimately, by the end of this workshop, you can create your own reports as a Markdown file or HTML file or pdf file to present it to your superiors.

:hushed::hushed::hushed:
```
=======================================
Get reports from whosoever is doing it
=======================================
```

You can achieve the following graphs and leave a good impression.

:astonished::astonished::scream:
```
=================================================
Get visualization graphs from whosoever is doing it
=================================================
```

## Introduction to Python and Jupyter Notebook

### Why Python ?

Python is a general purpose programming language that supports rapid development of scripts and applications.

![From StackOverflow Blog](https://zgab33vy595fw5zq-zippykid.netdna-ssl.com/wp-content/uploads/2017/09/growth_major_languages-1-1024x878.png)

Python’s main advantages:

* Open Source software, supported by Python Software Foundation
* Available on all platforms
* It is a general-purpose programming language
* Supports multiple programming paradigms
* Very large community with a rich ecosystem of third-party packages

### Jupyter Notebook as IDE for Python

We will be working with Python using Jupyter Notebook. This is a piece of software (also known as integrated development environment, IDE ) that makes working in Python much easier. 

:confused::confused::confused:
> How to open jupyter notebook in different platforms !!!

Now let's open Jupyter Notebook by typing `jupyter-notebook` in the terminal/console.

Jupyter Notebook opens in your default browser with a list of files and directories in the home directory with this URl `http://localhost:8888/tree`  

![](./First.png)

For this workshop, we will have all our files in `SWC_spring2018`. Navigate `Home-->Desktop-->SWC_spring2018-->Python_Basics` and hit New and click Python 3 to create a new file.

![](./Second.png)

:+1: Do it with students and make sure everyone is with you - put up red sticky notes if having problems, green when done with the task.

This opens up to the Notebook User Interface (UI). This has three areas.

* Menu 
* Toolbar
* Notebook area and cells

So if a cell is highlighted in `green` :green_heart:, it means the cell is in `edit mode`. If the cell is highlighted in `blue` :blue_heart:, it means the cell is in `command mode`.
 Now let us try the following commands one by one in `edit mode`. Type `3+5` and hit <kbd>Shift</kbd>+<kbd>Enter</kbd>

```python
            >>> 3+5
            >>> import math
            >>> math.sqrt(64) 
            >>> print("Welcome All !!!")
```

Similarly, we have interpreter mode in python which opens as follows

:confused::confused::confused:
> How to open python in different systems


### Interpreter Mode

Now let us see how interpreter mode works. Open a new tab in the terminal and type `python3` and hit enter.
This should open python in interpreter mode with `>>>` as shown.

![](./Third.png)

When you type commands in the terminal/console window and press 'ENTER', they are executed immediately and the output is displayed. Here are few examples:  

```python
            >>> 3+5
            >>> import math
            >>> math.sqrt(64) 
            >>> print("Welcome All !!!")
```
            
![](./Fourth.png)            

Symbol `>>>` means that the python is ready for the next command. If you enter incomplete commands, python will show SyntaxError or a Nameerror. 

## IDE for Python vs Interpreter Mode/Scripting Mode

Functionality is all the same. But the advantage of Jupyter Notebook is that it helps us write reports using Markdown file and supports in-text code blocks that are executed while rendering to HTML or pdf files.

![](./Fifth.png)

For this workshop we will be working with Jupyter Notebook. 

:+1: Do it with students and make sure everyone is with you - put up red sticky notes if having problems, green when done with the task.

**Now lets get started**

## 2. Building blocks of Python

Let's work in edit mode in Jupyter from now on so that you will have the record of all commands we used in this lesson.

### Variables/objects

One of the main concepts of any programming language is a notion of a variable. Variables are created to store values for future use.
To create a variable in python, use `=` as assignment operator:

```python
a = 5
print(a)
DNA = "ACTGATGCTAGC"
print(DNA)
```

**Challenge 2.1**
    
```python
=====
TASK: What will be the value of each  variable  after each statement in the following code?
=====
mass = 47.5
age = 122
mass = mass * 2.3
age = age - 20
height = height + 20      
```

As you can see, a variable is assigned a value equal to the value of the evaluated expression on the right side of the assignment operator. 

**A note on variable names:**
* NO SPACES in names
* DO NOT START with numbers
* Names should be MEANINGFUL - help yourself and others to understand your code! 

### Working with environment

#### List all variable defined in your environment

```python
who
```

#### Delete a specific variable in your environment

```python
del DNA
del a
```

#### To delete all the variables

```python
reset
```

### Functions

In general, a function takes an input and transforms it according to the function's definition(rules). You can recognize functions in python by the presence of parantheses. Objects in parantheses are called function's `arguments`.

#### Print is a widely used function

```python
DNA = "ATGCATGCT"
print(DNA)
```

- Here `print()` is a function.
- `(DNA)` is an argument to the function.

#### To Apply square root function

```python
import math
a = 64
math.sqrt(a)
sqrt_a = math.sqrt(a)
print(sqrt_a)
```

- `math` is the module which has square root function. A module is a collection of several related functions. 
- `sqrt()` is the function
- `(a)` is the argument to the function.
- The square root of the `a` is now assigned to a new variable named `sqrt_a`
- `print()` function takes `sqrt_a` as argument and displays it to the user.

### Help functions

Question mark followed by the name of the module/function provides information about the module.

```python
?math.sqrt()
```

### Present directory is given by

```python
pwd
```

### Data types and Data structures

Let's assign value of 45 to a variable `age`. We just created the smallest object in R:

```python
dna = "ATCGTCAC"

#some useful functions to know more about the object 
len(dna)

age = 45

#some useful functions to know more about the object 
a = str(age)
```

Variables can hold values of various types. Most common data types:

  * Int
  * Float
  * Str
  * Boolean

  
For example: What data type is stored in `score` variable?
```python
score = 79
type(score)
type(str(score))
```

Sometimes you will need to convert between data types. There are functions that do that:  
  * int()
  * float()
  * str()
  * bool()
  
The last expression in the above example of nested function. Nested functions are very common in python, but are very difficult to understand at first. You can always split nested function into a series of single function calls. Remember that the variable inside the most inner paranthesis is an argument(input)for the function that will be evaluated first.

**Challenge 2.1:* Learn how to read the output of nested help functions **

```python
TASK: Break the following expression into multiple single function calls.
You will need to assign the output of each function to a variable that
will serve as an input(argument) for the next function. 
What is the value of each variable? What does each function do? 
Assign: `score = 79`

type(str(type(float(score))))
```

The conversion between data types is not always possible - why? Let's see what happens here:

```python
score = 79
type(score)
type(str(score))
##################
dna = "TCAGTCGATC"
type(dna)
type(int(dna))
```

:worried::worried::worried:
> I can understand that the conversion is not possible. I also see a value error. But I dont understand `Why`. Why is it not converting?


### Data structures with multiple elements

The small objects can be combined to build larger objects. Look at the gapminder dataset again. Our smallest objects can be used to represent a single element in the dataset, like individual year, or individual country, but what would be the simplest object that you can make with multiple elements?

#### List

List is a data structure in python that supports different data types as a single list. Each value in the list is separated by comma (,) and is indexed. Indexing starts from 0.

For example:

```python
list = [5,6.7,"Texas"]
type(list)
```
 - Notice the use of square brackets.
 
 |list   |= |5 | 6.7 | "Texas" |
 |:----- |:-|:-|:----|:--------|
 ||From Left||
 |Index  |= |0 | 1   |  2      |
 ||From Right||
 |Index  |= |-3| -2  |  -1     |
 
```python
list = [5,6.7,"Texas"]
type(list[0])
type(list[1])
type(list[2])
```
Now if you wanted to change a value say 6.7 to 5.4, you can do that. This property of the list is called `**mutable property**`

```python
list = [5,6.7,"Texas"]
list[1] = 5.4
list
```
 
#### Tuple

Tuples are similar to list. They can hold different data types as a list of values separated by comma(,).

For example:

```python
tuple = (5,6.7,"Texas")
type(tuple)
```

 - Notice the use of simple brackets or parantheses.
 
 |tuple  |= |5 | 6.7 | "Texas" |
 |:----- |:-|:-|:----|:--------|
 ||From Left||
 |Index  |= |0 | 1   |  2      |
 ||From Right||
 |Index  |= |-3| -2  |  -1     |
 

Now if you wanted to change a value say 6.7 to 5.4, you **CANNOT** do that. This property of the tuples makes it `**immutable**`

```python
tuple = (5,6.7,"Texas")
tuple[1] = 5.4
```

```
---------------------------------------------------------------------------
TypeError                                 Traceback (most recent call last)
<ipython-input-91-6b513665c9a0> in <module>()
----> 1 tuple[1] = 5.4

TypeError: 'tuple' object does not support item assignment
```

#### Dictionary


#### Data Frame with Pandas
  
* Operators
  * "+"
  * "-"
  * "*"
  * "/"
  * "%"
  * ">"
  * ">="
  * "<"
  * "<="
  * "=="
  * "!="
  * in
  * not in
  
* Condition Statements
  * If
  * Else
  * Elif

* Looping 
  * while
  * for
  
* About python libraries

  * Importing the data using Pandas  
  * Viewing our dataframe
  * Statistics by Grouping using Pandas
  * Quick Summary using Pandas
  * Ploting of Summary using Pandas
