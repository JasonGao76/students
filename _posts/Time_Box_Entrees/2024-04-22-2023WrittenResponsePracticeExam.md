---
layout: post
title: 2023 Written Response Practice Exam 1
hide: true
comments: true
description: 
type: tangibles
courses: { compsci: {week: 28} }
---
> Written Response Practice Exam 1
- Component A: Program Code
    - See actual CB submission (CPT Program Code.pdf)

- Component B: Video
    - See actual CB submission (CPT Submission Video.mp4)

- Component C: Personalized Project Reference
    - See actual CB submission (420Y23W8_PPR.pdf)

- Question 1: Describe one piece of documentation that would be appropriate to include with or in your program. Describe the intended purpose of this documentation by identifying who would use it and what they would do with it.
    - Question: are we meant to actually have a piece of documentation or is it just if you were to have one, what would be appropriate?
    - One piece of documentation that would be appropriate to include in our program would be a rule book. My program is a game intended to help test and improve people's logical thinking to make predictions, so given that the player hopefully reads the rule book before playing, the rule book would help guide them in knowing what themselves and the enemy bot are allowed to do, helping them to properly play and better understand the game. 

- Question 2:
    - a. Consider the first iteration statement included in the Procedure section of your Personalized Project Reference. Describe the condition(s) that will cause the body of the iteration statement to execute at least once.
        - The body of the iteration statement will execute when the number passed through as an argument (number) is within the array (arr) also passed through as an argument, essentially checking if the inputted number is in the inputted array by going through each value in the array and seeing if it is equal to the number.

    - b. Consider the procedure identified in part (i) of the Procedure section of your Personalized Project Reference. Write a call to your procedure with specific argument(s) that you could use for testing this procedure. Describe the program functionality that is related to this call.
        - if (checkPosition(5, [1, 3, 4, 5])) {
            console.log("yay")
        }
        else {
            console.log("naur")
        }
        - This call's arguments reflect that of a user at position 2 trying to move to position 5. At position 2, the user (assuming regular movement) is able to move to the adjacent spaces of 1, 3, 4, or 5. If the user inputs position 5 to move to, this code will check to see if "5" is within the array of possible positions to move to, or "[1, 3, 4, 5]". This confirms if the user input is actually valid, and if so, will move the user to their inputted position, and if not, will give an error.
        - Alternatively, this could be used to see if the user attacking position 5 is within a valid spot to attack, or to see if the user is within the enemy bot's spaces to attack using the same logic.

    - c. Consider the list identified in the List section of your Personalized Project Reference. Explain how you would need to adjust this part of your program if the list was not included in your code.
        - If this dictionary of lists was not included in my code, I would have to define a new array of every position a spot can act on for that spot (for example, var position1 = [2, 3], var position2 = [1, 3, 4, 5], and so on) every time the user moves or attacks (movement() function and attack() function) and whenever the enemy bot acts within those functions as well. Getting the user input (or random number in the enemy bot's case) stays the same, but rather than using that value to get the positions they can act on through the dictionary, a series of if and else if functions would need to be used to check every position value to see if it matches the user or bot position, and then the corresponding array variable can be used. In the end, this would be much more bulky compared to using a dictionary.

> Written Response Practice Exam 2
- Components A, B, C: See above.

- Question 1: Explain how you used or could have used feedback, testing, or reflection in the development of your program.
    - I could've used feedback in the development of my program by asking my friends or family to try playing the game from the beginning without any input from me, which would help me figure out what parts are intuitive, what parts of the text are unclear, what features don't make sense to them, if there were loopholes or errors in the code that I didn't catch, what features they would like to see in the game, and more. This would then help guide me to edit the code, debug some errors, and include additional features.

- Question 2:
    - a. Consider the first conditional statement included in the Procedure section of your Personalized Project Reference. Write an equivalent Boolean expression for this conditional statement.
        - if (true) {
            document.getElementById("enemyalert").textContent = "The enemy is one step away from you! ";
            document.getElementById("actions").textContent = "move to or attack";
            return true;
        }
        else { // essentially if false
            document.getElementById("enemyalert").textContent = "";
            document.getElementById("actions").textContent = "move to";
        }
    - b. Consider the procedure identified in part (i) of the Procedure section of your Personalized Project Reference. Identify a strategy, other than using test cases, that you can use to test the correctness of your procedure. Describe how you would use this strategy.
        - One way, other than using test cases, to test the procedure's correctness is to use textual outputs such as console.log() in each step with a unique text output, as this would allow me to see which steps are properly running (displaying the output) and not (not displaying the output or displaying it when it shouldn't). I would put a console.log("for " + i) right after the for to check to see that each element in the array is being iterated through, a console.log("if " + i) under the if condition to see whether or not the code is properly checking the equivalence for the if condition, and lastly a console.log("else " + i) under the else condition to see if the code is properly handling the event that the if condition isn't met for the right numbers.
    - c. Consider the procedure identified in part (i) of the Procedure section of your Personalized Project Reference. Procedures are often used to organize larger problems into subproblems or smaller tasks. Identify the subproblem being solved or task that is being accomplished by your procedure. Explain how the procedure is used to accomplish the overall functionality of your program.
        - This procedure's task is to check whether or not a number that's passed through as an argument is within the array that's also passed through as an argument by iterating through each value in the array and checking if it is equivalent to the number passed through, updating the appropriate text display and returning a Boolean as well. This is useful whenever a check needs to be done to see if an inputted number is valid for the player's actions, ensuring that the game's rules are actually being enforced and that the player moves to and attacks the proper spaces.

> Written Response Practice Exam 3
- Components A, B, C: See above.

- Question 1: Describe the problem that your program was created to address or the creative expression it pursues.
    - 

- Question 2:
    - a. Consider the code segment in part (ii) of the List section of your Personalized Project Reference that shows how your list is being used. Explain in detailed steps how this code segment works. Your explanation must be detailed enough for someone else to write the code segment.
        - 
    - b. Consider the procedure identified in part (i) of the Procedure section of your Personalized Project Reference. Passing different values as arguments to a procedure can cause different segments of code to execute. Based on one of your arguments, describe where you could insert output statements in your procedure to test whether a block of code is executed or not. If it is not possible for different arguments to cause different segments of code to execute in your procedure, explain why not.
        - 
    - c. Consider the procedure identified in part (i) of the Procedure section of your Personalized Project Reference. Explain how your program could be written differently if one of your parameters was removed from your procedure.
        - 