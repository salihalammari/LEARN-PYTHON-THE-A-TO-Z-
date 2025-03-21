# 1.1 Section 1 – Introduction to Programming

Hello there, and welcome to section one! We will start off by learning about some of the universal concepts of programming, such as instruction list, source file, language elements, compilation and interpretation. Ready? Let's start!

### 1.1.1 How does a computer program work?

A program makes a computer usable. Without a program, a computer, even the most powerful one, is nothing more than an object. Similarly, without a player, a piano is nothing more than a wooden box.

Computers are able to perform very complex tasks, but this ability is not innate. A computer's nature is quite different.

It can execute only extremely simple operations. For example, a computer cannot understand the value of a complicated mathematical function by itself, although this isn't beyond the realms of possibility in the near future.

Contemporary computers can only evaluate the results of very fundamental operations, like adding or dividing, but they can do it very fast, and can repeat these actions virtually any number of times.

Imagine that you want to know the average speed you've reached during a long journey. You know the distance, you know the time, you need the speed.

Naturally, the computer will be able to compute this, but the computer is not aware of such things as distance, speed, or time. Therefore, it is necessary to instruct the computer to:

1. accept a number representing the distance;
2. accept a number representing the travel time;
3. divide the former value by the latter and store the result in the memory;
4. display the result (representing the average speed) in a readable format.

These four simple actions form a program. Of course, these examples are not formalized, and they are very far from what the computer can understand, but they are good enough to be translated into a language the computer can accept.

Language is the keyword.

### 1.1.2 Natural languages vs. programming languages

A language is a means (and a tool) for expressing and recording thoughts. There are many languages all around us. Some of them require neither speaking nor writing, such as body language; it's possible to express your deepest feelings very precisely without saying a word.

Another language you use each day is your mother tongue, which you use to manifest your will and to ponder reality. Computers have their own language, too, called machine language, which is very rudimentary.

A computer, even the most technically sophisticated, is devoid of even a trace of intelligence

### 1.1.3 What makes a language?

We can say that each language (machine or natural, it doesn't matter) consists of the following elements:

- **an alphabet**: a set of symbols used to build words of a certain language (e.g., the Latin alphabet for English, the Cyrillic alphabet for Russian, Kanji for Japanese, and so on)
- **a lexis**: (aka a dictionary) a set of words the language offers its users (e.g., the word "computer" comes from the English language dictionary, while "cmoptrue" doesn't; the word "chat" is present both in English and French dictionaries, but their meanings are different)
- **a syntax**: a set of rules (formal or informal, written or felt intuitively) used to determine if a certain string of words forms a valid sentence (e.g., "I am a python" is a syntactically correct phrase, while "I a python am" isn't)
- **semantics**: a set of rules determining if a certain phrase makes sense (e.g., "I ate a doughnut" makes sense, but "A doughnut ate me" doesn't)

### 1.1.4 Machine language vs. high-level language

The IL is, in fact, the alphabet of a machine language. This is the simplest and most primary set of symbols we can use to give commands to a computer. It's the computer's mother tongue.

Unfortunately, this mother tongue is a far cry from a human mother tongue. We both (computers and humans) need something else, a common language for computers and humans, or a bridge between the two different worlds.

We need a language in which humans can write their programs and a language that computers may use to execute the programs, one that is far more complex than machine language and yet far simpler than natural language.

Such languages are often called high-level programming languages. They are at least somewhat similar to natural ones in that they use symbols, words and conventions readable to humans. These languages enable humans to express commands to computers that are much more complex than those offered by ILs.

A program written in a high-level programming language is called a source code (in contrast to the machine code executed by computers). Similarly, the file containing the source code is called the source file.

### 1.1.5 Compilation vs. Interpretation

Computer programming is the act of composing the selected programming language's elements in the order that will cause the desired effect. The effect could be different in every specific case – it's up to the programmer's imagination, knowledge and experience.

Of course, such a composition has to be correct in many senses:

- **alphabetically** – a program needs to be written in a recognizable script, such as Roman, Cyrillic, etc.
- **lexically** – each programming language has its dictionary and you need to master it; thankfully, it's much simpler and smaller than the dictionary of any natural language;
- **syntactically** – each language has its rules and they must be obeyed;
- **semantically** – the program has to make sense.

Unfortunately, a programmer can also make mistakes with each of the above four senses. Each of them can cause the program to become completely useless.

Let's assume that you've successfully written a program. How do we persuade the computer to execute it? You have to render your program into machine language. Luckily, the translation can be done by a computer itself, making the whole process fast and efficient.

There are two different ways of transforming a program from a high-level programming language into machine language:

#### Compilation

Compilation – the source program is translated once (however, this act must be repeated each time you modify the source code) by getting a file (e.g., an .exe file if the code is intended to be run under MS Windows) containing the machine code. Now you can distribute the file worldwide; the program that performs this translation is called a compiler or translator.

#### Interpretation

Interpretation – you (or any user of the code) can translate the source program each time it has to be run. The program performing this kind of transformation is called an interpreter, as it interprets the code every time it is intended to be executed. It also means that you cannot just distribute the source code as-is, because the end-user also needs the interpreter to execute it.

Due to some very fundamental reasons, a particular high-level programming language is designed to fall into one of these two categories.

There are very few languages that can be both compiled and interpreted. Usually, a programming language is projected with this factor in its constructors' minds – will it be compiled or interpreted?

### 1.1.6 What does the interpreter do?

Let's assume once more that you have written a program. Now, it exists as a computer file: a computer program is actually a piece of text, so the source code is usually placed in text files.

Note: it has to be pure text, without any decorations like different fonts, colors, embedded images or other media. Now you have to invoke the interpreter and let it read your source file.

The interpreter reads the source code in a way that is common in Western culture: from top to bottom and from left to right. There are some exceptions - they'll be covered later in the course.

First of all, the interpreter checks if all subsequent lines are correct (using the four aspects covered earlier).

If the interpreter finds an error, it finishes its work immediately. The only result in this case is an error message.

### The concept of Interpretation

The interpreter will inform you where the error is located and what caused it. However, these messages may be misleading, as the interpreter isn't able to follow your exact intentions, and may detect errors at some distance from their real causes.

For example, if you try to use an entity of an unknown name, it will cause an error, but the error will be discovered in the place where it tries to use the entity, not where the new entity's name was introduced.

In other words, the actual reason is usually located a little earlier in the code, for example, in the place where you had to inform the interpreter that you were going to use the entity of the name.

If the line looks good, the interpreter tries to execute it (note: each line is usually executed separately, so the trio "read-check-execute" can be repeated many times - more times than the actual number of lines in the source file, as some parts of the code may be executed more than once).

It is also possible that a significant part of the code may be executed successfully before the interpreter finds an error. This is normal behavior in this execution model.

You may ask now: which is better? The "compiling" model or the "interpreting" model? There is no obvious answer. If there had been, one of these models would have ceased to exist a long time ago. Both of them have their advantages and their disadvantages.

### 1.1.7 Compilation vs. Interpretation – Advantages and Disadvantages

|   | Compilation  |  Interpretation |
|---|---|---|
| Advabtages  | the execution of the translated code is usually faster; only the user has to have the compiler - the end- user may use the use the code without it; the translated code is stored using machine language-as it is very hard to understand it, your own invention and programming tricks are likely to remain your secret | you can run the code as soon as you complete it - there are no additional phases of translation; the code is storedusing programming language-this means that it can be run on computers using different machine languages; you don't compile your code separately for each different architecture.  |
| Disadvantages | the compilation itself may be a very time- consuming process - you may not be able to run your code immediately after making an amendment; you have to have as many compilers as hardware platforms you want your code to be run on. | don't expect interpretation to ramp up your code to high speed- your code will share the computer's power with the interprter, so it can't be really fast; both you annd the end user have to have the interpreter to run your code  |

What does this all mean for you?

- Python is an interpreted language. This means that it inherits all the described advantages and disadvantages. Of course, it adds some of its unique features to both sets.

- If you want to program in Python, you'll need the Python interpreter. You won't be able to run your code without it. Fortunately, Python is free. This is one of its most important advantages.

Due to historical reasons, languages designed to be utilized in the interpretation manner are often called scripting languages, while the source programs encoded using them are called scripts. Okay, let's meet Python.

# 1.2 Section 2 – Introduction to Python

Welcome to section two. Here, we will learn a little bit about the history of Python, different Python versions and implementations, and the impact that Python has had on modern-day programming. Let's begin.

### 1.2.1 Python – a tool, not a reptile

What is Python?

Python is a widely-used, interpreted, object-oriented, and high-level programming language with dynamic semantics, used for general-purpose programming.

And while you may know the python as a large snake, the name of the Python programming language comes from an old BBC television comedy sketch series called Monty Python's Flying Circus.

At the height of its success, the Monty Python team were performing their sketches to live audiences across the world, including at the Hollywood Bowl.

Since Monty Python is considered one of the two fundamental nutrients to a programmer (the other being pizza), Python's creator named the language in honor of the TV show.

### 1.2.2 Who created Python?

One of the amazing features of Python is the fact that it is actually one person's work. Usually, new programming languages are developed and published by large companies employing lots of professionals, and due to copyright rules, it is very hard to name any of the people involved in the project. Python is an exception.

There are not many languages whose authors are known by name. Python was created by [Guido van Rossum](https://en.wikipedia.org/wiki/Guido_van_Rossum ), born in 1956 in Haarlem, the Netherlands. Of course, Guido van Rossum did not develop and evolve all the Python components himself...

The speed with which Python has spread around the world is a result of the continuous work of thousands (very often anonymous) programmers, testers, users (many of them aren't IT specialists) and enthusiasts, but it must be said that the very first idea (the seed from which Python sprouted) came to one head – Guido's.

### Python's Philosophy

Python's design philosophy emphasizes code readability and simplicity. The language's syntax is meant to be clear and expressive, allowing programmers to write code that is both easy to understand and maintain. This philosophy is encapsulated in "The Zen of Python," a collection of aphorisms that capture the guiding principles of Python's design.

To view "The Zen of Python," you can simply type `import this` in the Python interpreter. Some of the key principles include:

- Beautiful is better than ugly.
- Explicit is better than implicit.
- Simple is better than complex.
- Complex is better than complicated.
- Readability counts.

These principles help ensure that Python code is not only functional but also elegant and easy to read, making it a favorite among developers for both small scripts and large-scale applications.

### 1.2.3 A hobby programming project

The circumstances in which Python was created are a bit puzzling. According to Guido van Rossum:

> In December 1989, I was looking for a "hobby" programming project that would keep me occupied during the week around Christmas. My office (...) would be closed, but I had a home computer, and not much else on my hands. I decided to write an interpreter for the new scripting language I had been thinking about lately: a descendant of ABC that would appeal to Unix/C hackers. I chose Python as a working title for the project, being in a slightly irreverent mood (and a big fan of Monty Python's Flying Circus).  
> — Guido van Rossum

### Python goals

In 1999, Guido van Rossum defined his goals for Python:

- an easy and intuitive language just as powerful as those of the major competitors;
- open source, so anyone can contribute to its development;
- code that is as understandable as plain English;
- suitable for everyday tasks, allowing for short development times.

About 20 years later, it is clear that all these intentions have been fulfilled. Some sources say that Python is the most popular programming language in the world, while others claim it's the second or the third.

Either way, it still occupies a high rank in the top ten of the       [PYPL PopularitY of Programming Language](https://pypl.github.io/PYPL.html#google_vignette ) and the [TIOBE Programming Community Index](https://www.tiobe.com/tiobe-index/ ).

Python isn't a young language anymore. It is mature and trustworthy. It's not a one-hit wonder. It's a bright star in the programming firmament, and time spent learning Python is a very good investment.

### 1.2.4 What makes Python so special?

Why Python? How does it happen that programmers, young and old, experienced and novice, want to use it? How did it happen that large companies adopted Python and implemented their flagship products using it?

There are many reasons – we've listed some of them already, but let's enumerate them again in a more practical manner:

- **It's easy to learn** - the time needed to learn Python is shorter than for many other languages; this means that it's possible to start the actual programming faster.
- **It's easy to teach** - the teaching workload is smaller than that needed by other languages; this means that the teacher can put more emphasis on general (language-independent) programming techniques, not wasting energy on exotic tricks, strange exceptions and incomprehensible rules.
- **It's easy to use for writing new software** - it's often possible to write code faster when using Python.
- **It's easy to understand** - it's also often easier to understand someone else's code faster if it is written in Python.
- **It's easy to obtain, install and deploy** - Python is free, open and multiplatform; not all languages can boast that.

### 1.2.5 Python rivals?

Python has two direct competitors, with comparable properties and predispositions. These are:

- **Perl** – a scripting language originally authored by Larry Wall;
- **Ruby** – a scripting language originally authored by Yukihiro Matsumoto.

The former is more traditional and more conservative than Python, and resembles some of the old languages derived from the classic C programming language.

In contrast, the latter is more innovative and more full of fresh ideas than Python. Python itself lies somewhere between these two creations.

The Internet is full of forums with infinite discussions on the superiority of one of these three over the others, should you wish to learn more about each of them.

### 1.2.6 Where can we see Python in action?

We see it every day and almost everywhere. It's used extensively to implement complex Internet services like search engines, cloud storage and tools, social media and so on. Whenever you use any of these services, you are actually very close to Python, although you wouldn't know it.

Many developing tools are implemented in Python. More and more everyday-use applications are being written in Python. Lots of scientists have abandoned expensive proprietary tools and switched to Python. Lots of IT project testers have started using Python to carry out repeatable test procedures. The list is long.

### 1.2.7 Why not Python?

Despite Python's growing popularity, there are still some niches where Python is absent, or is rarely seen:

- **Low-level programming**: Sometimes called "close to metal" programming, if you want to implement an extremely effective driver or graphical engine, you wouldn't use Python.
- **Applications for mobile devices**: Although this territory is still waiting to be conquered by Python, it will most likely happen someday.

### 1.2.8 There is more than one Python

#### Python 2 vs. Python 3

There are two main kinds of Python, called Python 2 and Python 3.

Python 2 is an older version of the original Python. Its development has since been intentionally stalled, although that doesn't mean that there are no updates to it. On the contrary, the updates are issued on a regular basis, but they are not intended to modify the language in any significant way. They rather fix any freshly discovered bugs and security holes. Python 2's development path has reached a dead end already, but Python 2 itself is still very much alive.

Python 3 is the newer (or to be more precise, the current) version of the language. It's going through its own evolutionary path, creating its own standards and habits.

These two versions of Python aren't compatible with each other. Python 2 scripts won't run in a Python 3 environment and vice versa, so if you want the old Python 2 code to be run by a Python 3 interpreter, the only possible solution is to rewrite it, not from scratch, of course, as large parts of the code may remain untouched, but you do have to revise all the code to find all possible incompatibilities. Unfortunately, this process cannot be fully automatized.

It's too hard, too time-consuming, too expensive, and too risky to migrate an old Python 2 application to a new platform, and it's even possible that rewriting the code will introduce new bugs into it. It's easier, and more sensible, to leave these systems alone and to improve the existing interpreter, instead of trying to work inside the already functioning source code.

Python 3 isn't just a better version of Python 2 – it is a completely different language, although it's very similar to its predecessor. When you look at them from a distance, they appear to be the same, but when you look closely, though, you notice a lot of differences.

If you're modifying an old existing Python solution, then it's highly likely that it was coded in Python 2. This is the reason why Python 2 is still in use. There are too many existing Python 2 applications to discard it altogether.


  Note  
If you're going to start a new Python project, you should use Python 3, and this is the version of Python that will be used during this course.

It is important to remember that there may be smaller or bigger differences between subsequent Python 3 releases (e.g., Python 3.6 introduced ordered dictionary keys by default under the CPython implementation) – the good news, though, is that all the newer versions of Python 3 are backward compatible with the previous versions of Python 3. Whenever meaningful and important, we will always try to highlight those differences in the course.

All the code samples you will find during the course have been tested against Python 3.4, Python 3.6, Python 3.7, Python 3.8, and Python 3.9.
#### Key Differences

- **Print Statement**: In Python 2, `print` is treated as a statement, whereas in Python 3, it is a function.
    ```python
    # Python 2
    print "Hello, World!"
    
    # Python 3
    print("Hello, World!")
    ```

- **Integer Division**: In Python 2, dividing two integers performs floor division, while in Python 3, it performs true division.
    ```python
    # Python 2
    print 5 / 2  # Output: 2
    
    # Python 3
    print(5 / 2)  # Output: 2.5
    ```

- **Unicode**: In Python 2, strings are ASCII by default, whereas in Python 3, strings are Unicode by default.
    ```python
    # Python 2
    print type("Hello")  # Output: <type 'str'>
    
    # Python 3
    print(type("Hello"))  # Output: <class 'str'>
    ```

- **xrange**: In Python 2, `xrange()` is used for iterations, while in Python 3, `range()` behaves like `xrange()` and `xrange()` is removed.
    ```python
    # Python 2
    for i in xrange(5):
            print i
    
    # Python 3
    for i in range(5):
            print(i)
    ```

#### Migration

Migrating from Python 2 to Python 3 can be challenging due to these and other differences. However, tools like `2to3` can help automate much of the process. It's generally recommended to use Python 3 for new projects, as Python 2 has reached the end of its life and is no longer supported.

### 1.2.9 Python Implementations

Python has several implementations, each tailored for different use cases:

- **CPython**: The default and most widely-used implementation, written in C.
- **Jython**: An implementation of Python that runs on the Java platform.
- **MironPython**: An implementation of Python running on the .NET framework.
- **PyPy**: An implementation focused on speed, using a Just-In-Time (JIT) compiler.

Each implementation has its own strengths and weaknesses, and the choice of implementation can depend on the specific requirements of a project.

### 1.2.10 Python's Impact on Modern Programming

Python has had a significant impact on modern programming, influencing many other languages and becoming a staple in various fields such as web development, data science, artificial intelligence, and more. Its simplicity and readability have made it a popular choice for beginners and experienced developers alike.

Let's dive deeper into Python's ecosystem and explore some of the libraries and frameworks that have contributed to its success.

## 1.3 Section 3 – Downloading and Installing Python

Welcome to section three, where we will talk about the ways of obtaining, installing, and configuring Python on your local computer. This section is optional, as throughout the course you will be able to launch, test, and experiment with all your Python programs in Edube Interactive TM, the programming environment that we have integrated with the learning platform and these study resources. Still, if you can download and install Python on your local machine, we strongly recommend it.

### 1.3.1 Begin your Python journey

#### How to get Python and how to get to use it

There are several ways to get your own copy of Python 3, depending on the operating system you use.

#### For Linux Users

Linux users most probably have Python already installed - this is the most likely scenario, as Python's infrastructure is intensively used by many Linux OS components.

For example, some distributors may couple their specific tools together with the system and many of these tools, like package managers, are often written in Python. Some parts of graphical environments available in the Linux world may use Python, too.

If you're a Linux user, open the terminal/console, and type:

```sh
python3
```

at the shell prompt, press Enter and wait. If you see something like this:

```
Python 3.x.x (default, ... , ...)
[GCC ...] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>
```

then you don't have to do anything else.

If Python 3 is absent, then refer to your Linux documentation in order to find out how to use your package manager to download and install a new package – the one you need is named `python3` or its name begins with that.

#### For Non-Linux Users

All non-Linux users can download a copy at [https://www.python.org/downloads/](https://www.python.org/downloads/).

Follow the instructions on the website to download and install Python for your operating system. Once installed, you can verify the installation by opening a terminal or command prompt and typing:

```sh
python --version
```

or

```sh
python3 --version
```

You should see the version of Python that you installed.

#### Using Python

After installing Python, you can start using it by opening a terminal or command prompt and typing `python` or `python3`. This will open the Python interactive shell where you can start writing and executing Python code.

For example, you can try the following:

```python
print("Hello, Python!")
```

This should output:

```
Hello, Python!
```

Congratulations! You have successfully installed Python and written your first Python program.

### 1.3.2 How to download, install, and configure Python

Because the browser tells the site you've entered the OS you use, the only step you have to take is to click the appropriate Python version you want.

In this case, select Python 3. The site always offers you the latest version of it.

#### For Windows Users

1. Start the downloaded `.exe` file and follow all the steps.
2. Leave the default settings the installer suggests for now, with one exception - look at the checkbox named `Add Python 3.x to PATH` and check it.

This will make things easier.

#### For macOS Users

A version of Python 2 may already have been preinstalled on your computer, but since we will be working with Python 3, you will still need to download and install the relevant `.pkg` file from the Python site.

1. Download the `.pkg` file from the [Python site](https://www.python.org/downloads/).
2. Open the downloaded file and follow the installation instructions.

After installation, you can verify the installation by opening a terminal and typing:

```sh
python3 --version
```

You should see the version of Python that you installed.

#### For Linux Users

Refer to your Linux documentation to find out how to use your package manager to download and install a new package – the one you need is named `python3` or its name begins with that.

After installation, you can verify the installation by opening a terminal and typing:

```sh
python3 --version
```

You should see the version of Python that you installed.

#### Using Python

After installing Python, you can start using it by opening a terminal or command prompt and typing `python` or `python3`. This will open the Python interactive shell where you can start writing and executing Python code.

For example, you can try the following:

```python
print("Hello, Python!")
```

This should output:

```
Hello, Python!
```

Congratulations! You have successfully installed Python and written your first Python program.

### 1.3.3 Starting your work with Python

Now that you have Python 3 installed, it's time to check if it works and make the very first use of it.

This will be a very simple procedure, but it should be enough to convince you that the Python environment is complete and functional.

There are many ways of utilizing Python, especially if you're going to be a Python developer.

To start your work, you need the following tools:

- an editor which will support you in writing the code (it should have some special features, not available in simple tools); this dedicated editor will give you more than the standard OS equipment;
- a console in which you can launch your newly written code and stop it forcibly when it gets out of control;
- a tool named a debugger, able to launch your code step-by-step, which will allow you to inspect it at each moment of execution.

Besides its many useful components, the Python 3 standard installation contains a very simple but extremely useful application named IDLE.

IDLE is an acronym: Integrated Development and Learning Environment.

Navigate through your OS menus, find IDLE somewhere under Python 3.x and launch it. This is what you should see:

Python shell

### 1.3.4 Your very first program before your first program...

It is now time to write and run your first Python 3 program. It will be very simple, for now.

The first step is to create a new source file and fill it with code. Click File in the IDLE menu and choose New file.

As you can see, IDLE opens a new window for you. You can use it to write and amend your code.

This is the editor window. Its only purpose is to be a workplace in which your source code is treated. Do not confuse the editor window with the shell window. They perform different functions.

The editor window is currently untitled, but it's good practice to start work by naming the source file.

Click File (in the new window), then click Save as..., select a folder for the new file (the desktop is a good place for your first programming attempts) and chose a name for the new file.

Note: don't set any extension for the file name you are going to use. Python needs its files to have the .py extension, so you should rely on the dialog window's defaults. Using the standard .py extension enables the OS to properly open these files.

Now put just one line into your newly opened and named editor window.

The line looks like this:

```python
print("Hisssssss...")
```

You can use the clipboard to copy the text into the file.

We're not going to explain the meaning of the program right now. You'll find a detailed discussion in the next chapter.

Take a closer look at the quotation marks. These are the simplest form of quotation marks (neutral, straight, dumb, etc.) commonly used in source files. Do not try to use typographic quotes (curved, curly, smart, etc.), used by advanced text processors, as Python doesn’t accept them.

Save the file (File -> Save) and run the program (Run -> Run Module).

If everything goes okay and there are no mistakes in the code, the console window will show you the effects caused by running the program.

In this case, the program hisses.

Try to run it once again. And once more.

Now close both windows now and return to the desktop.

### 1.3.5 How to spoil and fix your code

Now start IDLE again.

Click File, Open, point to the file you saved previously and let IDLE read it in. Try to run it again by pressing F5 when the editor window is active. As you can see, IDLE is able to save your code and retrieve it when you need it again.

IDLE contains one additional and helpful feature.

First, remove the closing parenthesis. Then enter the parenthesis again. Your code should look like this:

```python
print("Hisssssss..."
```

Every time you put the closing parenthesis in your program, IDLE will show the part of the text limited with a pair of corresponding parentheses. This helps you to remember to place them in pairs.

Remove the closing parenthesis again. The code becomes erroneous. It contains a syntax error now. IDLE should not let you run it.

Try to run the program again. IDLE will remind you to save the modified file. Follow the instructions.

Watch all the windows carefully.

A new window appears – it says that the interpreter has encountered an EOF (end-of-file) although (in its opinion) the code should contain some more text.

The editor window shows clearly where it happened.

Fix the code now. It should look like this:

```python
print("Hisssssss...")
```

Run it to see if it "hisses" again.

Let's spoil the code one more time. Remove one letter from the word `print`. Run the code by pressing F5. What happens now? As you can see, Python is not able to recognize the instruction.

You may have noticed that the error message generated for the previous error is quite different from the first one.

This is because the nature of the error is different and the error is discovered at a different stage of interpretation.

The editor window will not provide any useful information regarding the error, but the console windows might.

The message (in red) shows (in the subsequent lines):

- the traceback (which is the path that the code traverses through different parts of the program – you can ignore it for now, as it is empty in such a simple code);
- the location of the error (the name of the file containing the error, line number and module name); note: the number may be misleading, as Python usually shows the place where it first notices the effects of the error, not necessarily the error itself;
- the content of the erroneous line; note: IDLE’s editor window doesn’t show line numbers, but it displays the current cursor location at the bottom-right corner; use it to locate the erroneous line in a long source code;
- the name of the error and a short explanation.

Experiment with creating new files and running your code. Try to output a different message to the screen, e.g., `roar!`, `meow`, or even maybe an `oink!`. Try to spoil and fix your code – see what happens.

## 1.4 Module 1 Completion – Module Test

### Module 1 Test

#### Question 1
What is a computer program?

- A) A set of instructions that a computer follows to perform a task.
- B) A physical component of a computer.
- C) A type of hardware.
- D) None of the above.

#### Question 2
Which of the following is NOT a characteristic of a high-level programming language?

- A) Similar to human languages.
- B) Easier for humans to read and write.
- C) Directly executed by the computer's hardware.
- D) Requires translation to machine language.

#### Question 3
What is the main difference between compilation and interpretation?

- A) Compilation translates the entire program at once, while interpretation translates the program line by line.
- B) Compilation is slower than interpretation.
- C) Interpretation translates the entire program at once, while compilation translates the program line by line.
- D) There is no difference.

#### Question 4
Who created Python?

- A) Larry Wall
- B) Yukihiro Matsumoto
- C) Guido van Rossum
- D) Dennis Ritchie

#### Question 5
Which of the following is a key principle of Python's design philosophy?

- A) Complex is better than complicated.
- B) Implicit is better than explicit.
- C) Ugly is better than beautiful.
- D) Readability doesn't count.

#### Question 6
What is the default implementation of Python?

- A) Jython
- B) CPython
- C) MironPython
- D) PyPy

#### Question 7
Which version of Python should you use for new projects?

- A) Python 2
- B) Python 3
- C) Both Python 2 and Python 3
- D) Neither Python 2 nor Python 3

#### Question 8
How can you view "The Zen of Python"?

- A) By typing `import zen` in the Python interpreter.
- B) By typing `import this` in the Python interpreter.
- C) By typing `import python` in the Python interpreter.
- D) By typing `import philosophy` in the Python interpreter.

#### Question 9
What is the command to check the installed version of Python?

- A) `python --check`
- B) `python --version`
- C) `python --info`
- D) `python --status`

#### Question 10
Which of the following is NOT a Python implementation?

- A) CPython
- B) Jython
- C) MironPython
- D) RubyPython

Good luck!

