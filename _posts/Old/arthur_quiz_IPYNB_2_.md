---

---

```python
import getpass # for getpass.getuser() to get username
import random # to randomize the order of the questions

print("Hi " + getpass.getuser()) 

correct = 0 # number of correct questions
i = 1 # used to iterate through the dictionary

questions = {
    "What python command will output to console?": "print",
    "What python command asks for input from the user?": "input",
    "What python command defines a function?": "def"
}

keys = list(questions.keys()) # sets the keys of a dictionary into a list
random.shuffle(keys) # shuffles the questions for funzies

letters = ['F', 'F', 'F', 'F', 'F', 'F', 'D', 'C', 'B', 'A', 'A']

# ask question
# input - the question and the question number
# output - the response to the question
def ask_question(question, i):
    print(f"Question{str(i)} : " + question) # asks Question (number): question
    msg = input() # sets msg as the response
    return msg

# compares the response to the answer
# input - the response and the answer
# output - 0 if incorrect, 1 if correct
def check_response(question, response):
    if questions[question] == response:
        print("correct")
        return 1
    else:
        print(f"incorrect, the answer was \"{questions[question]}\"") # gives user the answer
        return 0

for question in keys:
    response = ask_question(question, i)
    if check_response(question, response): # if correct
        correct += 1 # number of correct
    i += 1 # question number
    
print(f"score: {str(correct)}/{str(len(questions))} or {str(int(correct/len(questions)*100))}%") # correct / number of questions

print("letter grade: " + str(letters[int(correct/len(questions)*10)]))
```

    Hi arthurliu
    Question1 : What python command defines a function?
    def
    correct
    Question2 : What python command will output to console?
    print
    correct
    Question3 : What python command asks for input from the user?
    input
    correct
    score: 3/3 or 100%
    letter grade: A



```python

```
