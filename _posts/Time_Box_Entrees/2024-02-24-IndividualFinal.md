---
layout: post
title: Individual Final
hide: true
comments: true
description: Individual final for CPT Project and CSP Final, correlation to CPT showing how my features/pull requests map to CollegeBoard requirements
type: tangibles
courses: { compsci: {week: 23} }
---

## Personalized Project Reference
> Procedure: Capture and paste two program code segments you developed during the administration of this task that contain a student-developed procedure that implements an algorithm used in your program and a call to that procedure.
- i. The first-program code segment must be a student-developed procedure that:
    - Defines the procedure's name and return type (if necessary)
    - Contains and uses one or more parameters that have an effect on the functionality of the procedure
    - Implements an algorithm that includes sequencing, selection and iteration
- ii. The second program code segment must show where your student-developed procedure is being called in your program.

> List:	Capture and paste two program code segments you developed during the administration of this task that contain a list (or other collection type) being used to manage complexity in your program.
- i. The first program code segment must show how data have been stored in the list.
- ii. The second program code segment must show the data in the same list being used, such as creating new data from the existing data or accessing multiple elements in the list, as part of fulfilling the program's purpose.

## Written Response 1: Program, Design, Function, and Purpose
> CRD-2.A: Describe the purpose of a computing innovation.  
- The purpose of my program is to provide entertainment to the user while also strengthening their logical thinking and reasoning by having them predict where the AI could be in order to maximize their probability of winning.

> CRD-2.B: Explain how a program or code segment functions.  
- Using procedure as a reference, which is checkPosition
- checkPosition takes in two parameters called "number", which is an integer, and "arr", which is an array, and uses a for loop to iterate through the array to check if the number is within the array. It does this within the conditions for the for loop by defining a variable i as 0, and will keep running the nested code as long as the condition of i is less than the length of the array is fulfilled. After each iteration, 1 is added to the value of i. The nested code checks if the number is in the array by using the variable i as the index for the array and using an if condition to see if the number in the array at index i is equal to number given as an argument. If so, then it updates the HTML text with id "enemyalert" and "actions" with new text and ends the function. If not, the HTML text is reverted back to the default and the for loop continues.
- When calling this procedure using the variables "position" and "enemyspot", "position" is defined as the location where the player is and "enemyspot" is defined as an array of all the positions the bot enemy is able to act on (attack or move to). So when this procedure is called using these variables, it checks to see if "position" is in the array of "enemyspot", and if so, it updates the HTML text to notify the user that they are within range of the bit's actions and that they are able to hit the bot now.

> CRD-2.C: Identify input(s) to a program. 
- Using procedure checkPosition as a reference, the arguments to the procedure call are the variables "position", which is a number, and enemyspot, which is an "array".
- Using overall program, we take a user input in the movement and attack box and use getElementById with ID of the HTML box to get what the user inputted.

> CRD-2.D: Identify output(s) produced by a program. 
- Using procedure checkPosition, the output is changing the HTML text to alert the player if the enemy is close by
    - I could have it return a booleon True if the if condition is met in case

> CRD-2.E: Develop a program using a development process. 
- Our whole game is a program developed with a development process, both frontend and backend
- All the various functions (calculateDamage, checkPosition, enemychoice, enemychoice2, enemymove, enemyattack, movement, attack)

> CRD-2.F: Design a program and its user interface. 
- Milanote plan of a program and the frontend screens. 

> CRD-2.G: Describe the purpose of a code segment or program by writing documentation. 
- 


## Written Question 2(a): Algorithm Development
> CRD-2.B: Explain how a program or code segment functions.
- See written response 1

> AAP-2.E.b: Evaluate expressions that use relational operators (<, >, ==, etc).
- Using procedure checkPosition as a reference, say array contains 2 numbers. At first, i = 0 so i < arr.length as 0 < 2. Then i++ adds 1 to i so i = 1, and i < arr.length as 1 < 2. But next time 1 gets added to i, i = 2 so i < arr.length is not true.

> AAP-2.F.b: Evaluate expressions that use logic operators (and, or, not).
- 

> AAP-2.H.b: Determine the result of conditional statements.
- 

> AAP-2.J: Express an algorithm that uses iteration without using a programming language.
- 

> AAP-2.K.b: Determine the result or side effect of iteration statements.
- 

> AAP-2.L: Compare multiple algorithms to determine if they yield the same side effect or result.
- 

> AAP-2.M.a: Create algorithms.
- 

> AAP-2.M.b: Combine and modify existing algorithms.
- 


## Written Question 2(b): Errors and Testing
> CRD-2.I.a: Identify the error. 

> CRD-2.I.b: Correct the error. 

> CRD-2.J: Identify inputs and corresponding expected outputs or behaviors that can be used to check the correctness of an algorithm or program.

## Written Question 2(c): Data and Procedural Abstraction
> AAP-1.D.a: Develop data abstraction using lists to store multiple elements.  

> AAP-1.D.b: Explain how the use of data abstraction manages complexity in program code.  

> AAP-2.O.a: Write iteration statements to traverse a list. 

> AAP-2.O.b: Determine the result of an algorithm that includes list traversals.  

> AAP-3.B: Explain how the use of procedural abstraction manages complexity in a program. 
