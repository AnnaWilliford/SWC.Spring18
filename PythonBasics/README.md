Software Carpentry Workshop: Lesson1: Introduction to Python
===


SWC workshop, February 2018  
Instructor: Balan Ramesh  
Time: 3 hours  

---

Good morning!
Before we start working with python, let's make a folder where you will save all your work during this workshop.

Let's make a folder `SWC_spring2018` on your Desktop. We will be working with this folder for the next 2 days so it is better if you leave it on the Desktop where it is easily accesible. It also helps for everyone to have the folder in the same location as it will make it easier to navigate to your files when we start using command line interface later today.

- [x] Do it with students and make sure everyone is with you - put up red sticky notes if having problems, green when done with the task. 

Now let's download datasets (Data.zip) for the workshop and put it in `SWC_spring2018` folder.

[Dataset](https://raw.githubusercontent.com/AnnaWilliford/2017-11-11-UTA/gh-pages/workshop/SWC_fall2017/Data.zip)

When you unzip this file, you should have `Data` folder with `ByCountry` folder and `gapminder.txt` file in it.


Finally, let's make another folder called  'Python_basics' inside `SWC_spring2018` folder. This is where we will save all files for this lesson.

- [x] do it with students and make sure everyone is with you - put up red sticky notes if having problems, green when done with the task.


Now we are ready to work with Python.

### Learning objectives of this workshop

- Understand benefits of using Python
- Understand how to work with Jupyter Notebook
- Understand how to go get data from Excel to Python
- Understand building blocks of Python language
- Understand how to extract parts of the dataset
- Understand how to write simple Python scripts

Ultimately, by the end of this workshop, you can create your own reports as a Markdown file or HTML file or pdf file to present it to your superiors.

```
=======================================
Get reports from whosoever is doing it
=======================================
```

You can achieve the following graphs and leave a good impression on your higher officers.

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

> How to open jupyter notebook in different platforms !!!

Now let's open Jupyter Notebook by typing `jupyter-notebook` in the terminal/console.

Jupyter Notebook opens in your default browser with a list of files and directories in the home directory with this URl `http://localhost:8888/tree`  

![](./First.png)

For this workshop, we will have all our files in `SWC_spring2018`. Navigate `Home-->Desktop-->SWC_spring2018-->Python_Basics` and hit New and click Python 3 to create a new file.

![](./Second.png)

- [x] do it with students and make sure everyone is with you - put up red sticky notes if having problems, green when done with the task.

This opens up to the Notebook User Interface (UI). This has three areas.

* Menu 
* Toolbar
* Notebook area and cells

So if a cell is highlighted in `green`, it means the cell is in `edit mode`. If the cell is highlighted in `blue`, it means the cell is in `command mode`.

### Interpreter Mode

Now let us see how interpreter mode works. Open a new tab in the terminal and type `python3` and hit enter.
This should open python in interpreter mode with `>>>` as shown.
![](./Third.png)

When you type commands in the terminal/console window and press 'ENTER', they are executed immediately and the output is displayed. Here are few examples:  

            >>> 3+5
            >>> import math
            >>> math.sqrt(64) 
            >>> print("Welcome All !!!")
            
![](./Fourth.png)            

Symbol `>>>` means that the python is ready for the next command. If you enter incomplete commands, python will show SyntaxError or a Nameerror. 

## IDE for Python vs Interpreter Mode/Scripting Mode

Functionality is all the same. But the advantage of Jupyter Notebook is that it helps us write reports using Markdown file and supports in-text code blocks that are executed while rendering to HTML or pdf files.

![](./Fifth.png)


Dataset

Examples and Challenges

* Variable

* Data Types
  * Int
  * Float
  * Str
  * Boolean

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
  
* Data Structures
  * List
  * Tuple
  * Dictionary
  * Data Frame with Pandas
  
* Functions

* About python libraries

  * Importing the data using Pandas  
  * Viewing our dataframe
  * Statistics by Grouping using Pandas
  * Quick Summary using Pandas
  * Ploting of Summary using Pandas
  
  
  
  
  
