import random

while True:

    print("=============================================================================PYTHON TUTORIAL============================================================================")
    print("Welcome to Python Tutorial! Come Learn Python in a fun way!")
    print("""Kindly Choose a lesson you want to learn below:
    
             For Prelim Lessons  : 1 for Introduction to Programming
                                   2 for Python Basic Syntax
                                   3 for Arithmetic Operators and Expressions
                                   4 for Basic Input and Output in Python
             For Midterm Lessons : 5 for Conditional Statements in Python
                                   6 for Logical Operator 
             For Finals Lesson   : 7 for Introduction to Iteration and Loops""")
    print("")         
    lesson = int(input("Choose a lesson (0 to exit): "))

    # EXIT
    if lesson == 0:
        print("THANK YOU FOR USING PYTHON TUTORIAL!")
        break

    # LESSONS
    elif lesson == 1:
        print("""
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------
                                                                           INTRODUCTION TO PROGRAMMING
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------
        PROGRAMMING LANGUAGE is a special language that computers understand and use to perform tasks.
        COMMON PROGRAMMING LANGUAGES includes PYTHON, C/C++, PHP, JAVA, JAVASCRIPT, RUBY
        
        PYTHON is a widely used programming language that was created by GUIDO VAN ROSSUM (a DUTCH SOFTWARE engineer) in 1991.
        It is also a high-level, interpreted, and general-purpose 
        programming language designed to be simple, readable, and easy to learn.
        
        WHY LEARN PYTHON?
        * Simple and Easy to Learn - Great for beginners
        * Readable Syntax - Code looks almost like english
        * Versatile Used in many fields- 
        * Huge Community - Lots of support, tutorials, and libraries
        
        To start Python programming you need the following:
        Professional IDES / CODE EDITORS such as PYCHARM, VISUAL STUDIO VODE, JUPYTER NOTEBOOK / JUPYTERLAB
        
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------""")
        activity = input("Do you want to take an activity? (Y) or (N):"). upper()
        print("")
        if activity == "Y":
            print("LET'S NOW TEST YOUR KNOWLEDGE!!!")
        else:
            print("Exit")
            break
                
        print("")
        
        
        words = { "python": "A programming language", "guido van rossum": "He created Python and is a dutch engineer", "programming language": "A special language that computers understand", 
             "pycharm": "This is one of those that you need to start Python programming", "java" : "It is included in the common programming languages"  }

        words_list = list(words.items())
        random.shuffle(words_list)
 
        for word, hint in words_list:
             print(f"\nHint: {hint} ({len(word)} letters)")
             for i in range(3, 0, -1):
                 if input(f"Guess ({i} left): ").strip() == word:
                     print("Correct!")
                     break
             else:
                 print(f"Wrong Answer! It was {word}.")
                 

    elif lesson == 2:
        print("""
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------
                                                                            PYTHON BASIC SYNTAX
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------
        SYNTAX refers to the set of rules that tells us how to correctly write a program in Python.
        
        PYTHON SYNTAX
        1. Python is Case sensitive - It treats uppercase and lowercase letters differently.
        2. Indentation - Unlike other programming languages. Python uses indentation (spaces) to define blocks of code.
        
        PRINTING OUTPUT
        
        The print() function displays information on the screen.
        TEXT (also called a string) must be enclosed in quotation marks, but you can print NUMBERS directly without quotation marks.
        
        PYHTON COMMENTS
        
        COMMENTS are IGNORED by Python because they are used to explain the code.
        
        VARIABLES, CONSTANTS, and DATA TYPES in PYTHON
        
        A VARIABLE is a name storage location used to keep data in a program. The value of a VARIABLE can change while the program is running.
        for example: a, b, c, age, name
        
        Rules for naming variables:
        * A variable  can have a short or a more descriptive name.
        * A variable name must start with a letter or the underscore character. It cannot start with a number.
        * Variable names are case sensitive. e.g (age and AGE are two different variables)
        
        Assigned Value to Variable
        In programming, we store data in variables. We assign a value to a variable using the = (assignment operator).
        
        Output Variables
        The python print() function is often used to output variables. In the print() function, you output multiple variables, separated by a comma and plus sign.
        
        BASIC DATA TYPES IN PYTHON
        
        Data Types are categories that tell python what kind of data a variable stores.
        
        Four Types of Data:
        * int - used for whole numbers
        * float - used for numbers with a decimal point
        * str - used for text or characters
        * bool - represents two things: True or False
         
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------""")
        
        activity = input("Do you want to take an activity? (Y) or (N):"). upper()
        print("")
        if activity == "Y":
            print("LET'S NOW TEST YOUR KNOWLEDGE!!!")
        else:
            print("Exit")
            break
            
        print("")
        
        words = { "syntax": "Set of rules", "indentation": "Used to define blocks of code", "print": "Displays information on the screen", "text": "Must be enclosed in quotation marks",
             "variable": "Used to keep data in a program", "int": "Used for whole numbers", "float": "For numbers with a decimal point", "str": "Used for text", "bool": "Either true or false"}

        words_list = list(words.items())
        random.shuffle(words_list)
 
        for word, hint in words_list:
             print(f"\nHint: {hint} ({len(word)} letters)")
             for i in range(3, 0, -1):
                 if input(f"Guess ({i} left): ").strip() == word:
                     print("Correct!")
                     break
             else:
                 print(f"Wrong Answer! It was {word}.")

    elif lesson == 3:
        print("""
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------
                                                                            ARITHMETIC OPERATORS AND EXPRESSIONS
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------
        ARITHMETIC OPERATORS are symbols used to perform mathematical calculations on numbers. They work the same way as the operators used everyday in mathematics.
        
        PYTHON ARITHMETIC OPERATORS are the following:
        + Addition - adds two values
        - Subtraction - subtracts the second value from the first
        * Multiplication - multiplies two values
        / Division - divides two values and returns a decimal
        // Floor Division - divides two values and returns the whole number part 
        % Modulus - returns the remainder of the division
        ** Exponentation - raises the first value to the power of the second
        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
        EXPRESSIONS IN PYTHON
        An expression is a combination of values, variables, and operators that evaluates to a result.
        
        Python follows the order of operations (PEMDAS): Parentheses, Exponents, Multiplication, Division, Addition, and Subtraction.
        
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------""")
        
        activity = input("Do you want to take an activity? (Y) or (N):"). upper()
        print("")
        if activity == "Y":
            print("LET'S NOW TEST YOUR KNOWLEDGE!!!")
        else:
            print("Exit")
            break
            
        print("")
        
        words = { "arithmetic operators": "Used to perform mathematical calculations", "addition": "Adds two values", "subtraction": "substract two values", "multiplication": "multiplies two values",
             "expression": "A combination of values, variables, etc." }

        words_list = list(words.items())
        random.shuffle(words_list)
 
        for word, hint in words_list:
             print(f"\nHint: {hint} ({len(word)} letters)")
             for i in range(3, 0, -1):
                 if input(f"Guess ({i} left): ").strip() == word:
                     print("Correct!")
                     break
             else:
                 print(f"Wrong Answer! It was {word}.")

    elif lesson == 4:
        print("""
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------
                                                                             BASIC INPUT AND OUTPUT IN PYTHON
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------
        ACCEPTING USER INPUT
        The purpose of input in programming is for real-life analogies (e.g., asking for a user's name and responding)
        
        * Using input() function
        * Syntax: variable = input("Message")
        * All input is string type by default
        
        For Formatting Output, you have to use comma , in print()
        
        CONVERTING INPUT TO OTHER DATA TYPES
        a. Float Input (for decimal numbers
        CODE:   grade = float(input("Enter your grade:")) 
                print(f"Your grade is {grade}) 
                
        b. Boolean input (True or False using conditions)
        CODE:   answer = input("Are you a student? (yes/no):")
                is_student = answer.lower() === "yes"
                print("Student status:", is-student) 
                
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------""")
        
        activity = input("Do you want to take an activity? (Y) or (N):"). upper()
        print("")
        if activity == "Y":
            print("LET'S NOW TEST YOUR KNOWLEDGE!!!")
        else:
            print("Exit")
            break
            
        print("")
            
        words = { "real-life analogies": "The purpose of input in programming", "comma": "You have to use this for formating output", "float input": "This is used for decimal numbers", "boolean input": "Used for true or false condition" }

        words_list = list(words.items())
        random.shuffle(words_list)
 
        for word, hint in words_list:
             print(f"\nHint: {hint} ({len(word)} letters)")
             for i in range(3, 0, -1):
                 if input(f"Guess ({i} left): ").strip() == word:
                     print("Correct!")
                     break
             else:
                 print(f"Wrong Answer! It was {word}.")
                 

    elif lesson == 5:
        print("""
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------
                                                                             CONDITIONAL STATEMENTS IN PYTHON
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------
        Introduction to Conditional Staments in Python
        A conditional statement allows a program to make decisions based on wether a condition is True or False.
        
        if - The if keyword starts the conditional statement.
        condition - The condition is evaluated. If it is True, the indented statement is executed.
        statement - The statement is the code that runs when the condition is True.
        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
        Relational Operators
        Also called as comparison operators, are used to compare two values. The result is always either TRue or False.
        
        (==) Equal to
        (!=) Not equal to
        (>) Greater than
        (<) Less than 
        (>=) Greater than or equal to
        (<=) less than or equal to
        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
        The if Statement
        The if statement executes a block of code only when a condition is true.
        
        if - The if keyword starts the statement.
        condition - The condition is avaluated. If it is True , the indented block is executed.
        statements - One or more statements that run when the condition is True.
        If the condition is False, the indented block is skipped.
        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~`
        The if-else Statement
        The else statement provides an alternative when the if condition is False.
        
        Key points:
        * Use else when you want an alternative action if the if condition is False.
        * Only one of the if or else block will be executed.
        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
        The if-elif-else Statement
        The elif statement is used when there are multiple conditions to evaluate. Python checks each condition from top to bottom and executes the first condition 
        that is True.
        
        Key points: 
        * Python checks conditions from top to bottom
        * If a condition is True, its block is executed and the rest are skipped.
        * If none of the conditions are Truues, the else block is executed.
        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
        Nested Condition in Python
        A nested condition is a condition inside another condition.
        
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------""")
        
        activity = input("Do you want to take an activity? (Y) or (N):"). upper()
        print("")
        if activity == "Y":
            print("LET'S NOW TEST YOUR KNOWLEDGE!!!")
        else:
            print("Exit")
            break
            
        print("")
            
        words = { "conditional statement": "Allows a program to make a decision", "if": "Starts the conditional statement", "statement": "It runs when the condition is true", "relational operators": "It is used to compare two values",
             "nested condition": "A condition inside another condition" }

        words_list = list(words.items())
        random.shuffle(words_list)
 
        for word, hint in words_list:
             print(f"\nHint: {hint} ({len(word)} letters)")
             for i in range(3, 0, -1):
                 if input(f"Guess ({i} left): ").strip() == word:
                     print("Correct!")
                     break
             else:
                 print(f"Wrong Answer! It was {word}.")

    elif lesson == 6:
        print("""
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------
                                                                             LOGICAL OPERATOR
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------
        What Are Logical Operators?
        Logical Operators are used to combine or reverse conditions in a python program. They are commonly used with if-elif-else.
        
        Logical Operators are the following:
                                            and - both conditions MUST be true
                                            or - at least ONE condition must be true
                                            not - REVERSES the result
                                            
        < The and operator returns True only when ALL conditions are True.
        < The or operator returns True when at least ONE conditions is True.
        < The not operator reverses the result of a condition.                                    
        
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------""")
        
        activity = input("Do you want to take an activity? (Y) or (N):"). upper()
        print("")
        if activity == "Y":
            print("LET'S NOW TEST YOUR KNOWLEDGE!!!")
        else:
            print("Exit")
            break
            
        print("")
            
        words = { "logical operators": "It is used to combine or reverse conditions", "and": "All conditions must be true ", "or": "One condition must be true", "not": "Reverses a condition" }

        words_list = list(words.items())
        random.shuffle(words_list)
 
        for word, hint in words_list:
             print(f"\nHint: {hint} ({len(word)} letters)")
             for i in range(3, 0, -1):
                 if input(f"Guess ({i} left): ").strip() == word:
                     print("Correct!")
                     break
             else:
                 print(f"Wrong Answer! It was {word}.")

    elif lesson == 7:
        print("""
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------
                                                                             INTRODUCTION TO ITERATION AND LOOPS
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------
        Iteration means repeating a process. In programming, it means repeatedly executing a set of instructions. Each repetition is called an iteration.
        It allows a program to perform the same task multiple times.
        
        Without a loop, instructions must be written repeatedly:
        
        Without loop:                                              Using loop:
                     print("Study Python")                                    for number in range(4):
                     print("Study Python")                                        print("Study Python")
                     print("Study Python")
                     print("Study Python")
        
        Both programs produce the same output, but the loop makes the program shorter and easier to modify.
        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
        Types of Loops in Python: It has two main types of loops; for and while.
        
        * for loop - repeats instructions for each item in a sequence. It is useful when the number of repetitions is known.
        * while loop - Repeats instructions while a condition is True. It is useful when repetition depends on a condition.
        
        ----------------------------------------------------------------------------------------------------------------------------------------------------------------""")
        
        activity = input("Do you want to take an activity? (Y) or (N):"). upper()
        print("")
        if activity == "Y":
            print("LET'S NOW TEST YOUR KNOWLEDGE!!!")
        else:
            print("Exit")
            break
            
        print("")
            
        words = { "iteration": "repeating a process", "loop": "Makes the program shorter", "for loop": "Useful for numbers", "while loop": "Useful when using a condition" }

        words_list = list(words.items())
        random.shuffle(words_list)
 
        for word, hint in words_list:
             print(f"\nHint: {hint} ({len(word)} letters)")
             for i in range(3, 0, -1):
                 if input(f"Guess ({i} left): ").strip() == word:
                     print("Correct!")
                     break
             else:
                 print(f"Wrong Answer! It was {word}.")

    else:
        print("Invalid lesson number!")
        continue

    # CONTINUE QUESTION
    print("")
    proceed = input("Do you want to proceed to another lesson? (Y) or (N): ").upper()

    if proceed == "Y":
        print("Returning to the main menu...")

    elif proceed == "N":
        print("THANK YOU FOR USING PYTHON TUTORIAL!")
        break

    else:
        print("Invalid answer! Exiting the program.")
        break       
