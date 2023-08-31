---
layout: default
title: Python Quiz
---



```python
# import useful commands
import sys
import getpass

# counter for end score
correctanswer = 0
wronganswer = 0
totalanswer = 0

# each question is defined as a separate function
# question 1
def question1():
    global correctanswer
    global wronganswer
    global totalanswer
    # global ___ is supposed to make the thing work and not give the local variable referenced before assignment error but it aint workin
    answertoq1 = input("Question 1: What is Python's output command?")
    if answertoq1.lower() == "print":
        print("You answered " + answertoq1 + ". This is correct. Well done.")
        correctanswer += 1
        totalanswer += 1
        return correctanswer and totalanswer
    else:
        print("You answered " + answertoq1 + ". Incorrect.")
        wronganswer += 1
        totalanswer += 1
        return wronganswer and totalanswer

# question 2
def question2():
    global correctanswer
    global wronganswer
    global totalanswer
    answertoq2 = input("What is the Python command to define a function?")
    if answertoq2.lower() == "def":
        print("You answered " + answertoq2 + ". This is correct. Well done.")
        correctanswer += 1
        totalanswer += 1
        return correctanswer and totalanswer
    else:
        print("You answered " + answertoq2 + ". Incorrect.")
        wronganswer += 1
        totalanswer += 1
        return wronganswer and totalanswer

# question 3
def question3():
    global correctanswer
    global wronganswer
    global totalanswer
    answertoq3 = input("What is the Python command to get a user input?")
    if answertoq3.lower() == "input":
        print("You answered " + answertoq3 + ". This is correct. Well done.")
        correctanswer += 1
        totalanswer += 1
        return correctanswer and totalanswer
    else:
        print("You answered " + answertoq3 + ". Incorrect.")
        wronganswer += 1
        totalanswer += 1
        return wronganswer and totalanswer

# question 4
def question4():
    global correctanswer
    global wronganswer
    global totalanswer
    answertoq4 = input("What is the parameter that a function takes called?")
    if answertoq4.lower() == "prompt" or answertoq4.lower() == "argument":
        print("You answered " + answertoq4 + ". This is correct. Well done.")
        correctanswer += 1
        totalanswer += 1
        return correctanswer and totalanswer
    else:
        print("You answered " + answertoq4 + ". Incorrect.")
        wronganswer += 1
        totalanswer += 1
        return wronganswer and totalanswer

# question 5
def question5():
    global correctanswer
    global wronganswer
    global totalanswer
    answertoq5 = input("What command is used to import libraries or functions?")
    if answertoq5.lower() == "import":
        print("You answered " + answertoq5 + ". This is correct. Well done.")
        correctanswer += 1
        totalanswer += 1
        return correctanswer and totalanswer
    else:
        print("You answered " + answertoq5 + ". Incorrect.")
        wronganswer += 1
        totalanswer += 1
        return wronganswer and totalanswer

# question 6
def question6():
    global correctanswer
    global wronganswer
    global totalanswer
    answertoq6 = input("What are two or more lines of code called?")
    if answertoq6.lower() == "sequence":
        print("You answered " + answertoq6 + ". This is correct. Well done.")
        correctanswer += 1
        totalanswer += 1
        return correctanswer and totalanswer
    else:
        print("You answered " + answertoq6 + ". Incorrect.")
        wronganswer += 1
        totalanswer += 1
        return wronganswer and totalanswer

# question 7
def question7():
    global correctanswer
    global wronganswer
    global totalanswer
    answertoq7 = input("What symbol concatenates strings?")
    if answertoq7.lower() == "+":
        print("You answered " + answertoq7 + ". This is correct. Well done.")
        correctanswer += 1
        totalanswer += 1
        return correctanswer and totalanswer
    else:
        print("You answered " + answertoq7 + ". Incorrect.")
        wronganswer += 1
        totalanswer += 1
        return wronganswer and totalanswer

# question 8
def question8():
    global correctanswer
    global wronganswer
    global totalanswer
    answertoq8 = input("Fill in the blanks, use no commas and place one space between your answers. __ and ____ commands are used to check if your answer to this question is correct.")
    if answertoq8.lower() == "if else":
        print("You answered " + answertoq8 + ". This is correct. Well done.")
        correctanswer += 1
        totalanswer += 1
        return correctanswer and totalanswer
    else:
        print("You answered " + answertoq8 + ". Incorrect.")
        wronganswer += 1
        totalanswer += 1
        return wronganswer and totalanswer

# question 9
def question9():
    global correctanswer
    global wronganswer
    global totalanswer
    answertoq9 = input("What function is used to turn numbers into strings?")
    if answertoq9.lower() == "str()" or answertoq9.lower() == "str":
        print("You answered " + answertoq9 + ". This is correct. Well done.")
        correctanswer += 1
        totalanswer += 1
        return correctanswer and totalanswer
    else:
        print("You answered " + answertoq9 + ". Incorrect.")
        wronganswer += 1
        totalanswer += 1
        return wronganswer and totalanswer

# question 10
def question10():
    global correctanswer
    global wronganswer
    global totalanswer
    answertoq10 = input("What two symbols and one number are used to add one to a numerical variable in the form: var ___?")
    if answertoq10.lower() == "+= 1" or answertoq10.lower() == "+=1":
        print("You answered " + answertoq10 + ". This is correct. Well done.")
        correctanswer += 1
        totalanswer += 1
        return correctanswer and totalanswer
    else:
        print("You answered " + answertoq10 + ". Incorrect.")
        wronganswer += 1
        totalanswer += 1
        return wronganswer and totalanswer

# question 11
def question11():
    global correctanswer
    global wronganswer
    global totalanswer
    answertoq11 = input("This text, used using the print command and quotations, is what type of text?")
    if answertoq11.lower() == "static" or answertoq11.lower() == "static text":
        print("You answered " + answertoq11 + ". This is correct. Well done.")
        correctanswer += 1
        totalanswer += 1
        return correctanswer and totalanswer
    else:
        print("You answered " + answertoq11 + ". Incorrect.")
        wronganswer += 1
        totalanswer += 1
        return wronganswer and totalanswer

# gradecalculator function
def gradecalculator():
    percentcorrect = round(100 * correctanswer / totalanswer,1)
    percentwrong = round(100 * wronganswer / totalanswer,1)
    if percentcorrect >= 90:
        print("You got %s out of %s right and %s out of %s wrong." % (correctanswer, totalanswer, wronganswer, totalanswer))
        print("This corresponds to %s percent correct and %s percent wrong." % (percentcorrect, percentwrong))
        print("You earned an A!")
    if percentcorrect >= 80 and percentcorrect < 90:
        print("You got %s out of %s right and %s out of %s wrong." % (correctanswer, totalanswer, wronganswer, totalanswer))
        print("This corresponds to %s percent correct and %s percent wrong." % (percentcorrect, percentwrong))
        print("You earned an B!")
    if percentcorrect >= 70 and percentcorrect < 80:
        print("You got %s out of %s right and %s out of %s wrong." % (correctanswer, totalanswer, wronganswer, totalanswer))
        print("This corresponds to %s percent correct and %s percent wrong." % (percentcorrect, percentwrong))
        print("You earned an C.")
    if percentcorrect >= 60 and percentcorrect < 70:
        print("You got %s out of %s right and %s out of %s wrong." % (correctanswer, totalanswer, wronganswer, totalanswer))
        print("This corresponds to %s percent correct and %s percent wrong." % (percentcorrect, percentwrong))
        print("You earned an D.")
    if percentcorrect >= 0 and percentcorrect <60:
        print("You got %s out of %s right and %s out of %s wrong." % (correctanswer, totalanswer, wronganswer, totalanswer))
        print("This corresponds to %s percent correct and %s percent wrong." % (percentcorrect, percentwrong))
        print("You earned an F.")

# the actual quiz; it asks whether or not user wants to take quiz, gives questions and runs grade calculatiosn if yes, ends if no
yesno = input("Welcome, " + str(getpass.getuser()) + ", to this quiz. Would you like to test yourself?")
if yesno.lower() == "yes":
    print("Good. Proceed.")
    question1()
    question2()
    question3()
    question4()
    question5()
    question6()
    question7()
    question8()
    question9()
    question10()
    question11()
    gradecalculator()
else:
    print("Goodbye.")
    # "sys.exit()" isnt working, try to find another way to exit system. arthur suggested "except SystemExist:" but didnt work but maybe try more
    # but its not really needed tbf, can just end at print
    # would be funny if it ran like make clean or something
```

    Good. Proceed.
    You answered print. This is correct. Well done.
    You answered def. This is correct. Well done.
    You answered inout. Incorrect.
    You answered argument. This is correct. Well done.
    You answered import. This is correct. Well done.
    You answered sequence. This is correct. Well done.
    You answered +. This is correct. Well done.
    You answered if else. This is correct. Well done.
    You answered str. This is correct. Well done.
    You answered +=1. This is correct. Well done.
    You answered static. This is correct. Well done.
    You got 10 out of 11 right and 1 out of 11 wrong.
    This corresponds to 90.9 percent correct and 9.1 percent wrong.
    You earned an A!
