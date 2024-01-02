---
toc: true
comments: false
layout: post
title: 2023 Written Response Practice Exam 1 Planning
description: Planning for CPT project using Collegeboard 2023 Written Response Practice Exam 1 and Binary Project
type: tangibles
courses: { compsci: {week: 18} }
---

## 2023 Written Response Practice Exam 1 Answering using Binary Project
> Question 1:
- Component A: Program Code <img src="https://i.postimg.cc/br477W5q/Question1-Component-A.jpg">
    - Note that I only included the parts I worked on.
    - <img src="https://i.postimg.cc/bvPFGMFF/Answer1-Question1-Component-A.jpg">
    - <img src="https://i.postimg.cc/xCTx5mQv/Answer2-Question1-Component-A.jpg">
    - <img src="https://i.postimg.cc/52dsGT1N/Answer3-Question1-Component-A.jpg">
    - <img src="https://i.postimg.cc/J0sTVWGt/Answer4-Question1-Component-A.jpg">
    - <img src="https://i.postimg.cc/MTPsFGZh/Answer5-Question1-Component-A.jpg">
    - <img src="https://i.postimg.cc/WbJ95jBH/Answer6-Question1-Component-A.jpg">
    - <img src="https://i.postimg.cc/MHg9zrQ5/Answer7-Question1-Component-A.jpg">
    - I do have input from a user to answer the question as seen in the first screenshot with the input tag. I do have at least one list, one of them being imageArray. I do have at least one procedure, one being called checkQuiz() that has a proper name (it checks the quiz) and it does not necessarily need a return since the output is within the procedure, but none of my procedures take in a parameter. I do have an algorithm with selection but not iteration in the checkQuiz() procedure as it selects a key in the dictionary answerKey to get the answer (value). The function is called in the .html file with the two buttons. There is an output based on the input and program as seen with resultContainer and correctAnswers and wrongAnswers output.
- Component B: Video <img src="https://i.postimg.cc/1RT1VV3b/Question1-Component-B.jpg">
    - My submission in the Binary Project video actually has a showcase of the quiz running and working in it with no narration and only subtitles, so that video actually works for this! Here is a version of the video only showing the showcase: https://drive.google.com/file/d/1C1Tc8bWw-YjIysmgijaT2JhI7Y8YTHT0/view?usp=sharing
    - Note that I could have made it longer and easier to see if I wanted to, but the core functionality and program remains the same.
- Component C: Personalized Project Reference <img src="https://i.postimg.cc/jSHp184r/Question1-Component-C.jpg">
    - Same as Question 2, so see Question 2.
- Question <img src="https://i.postimg.cc/02wRY56j/Question1-Question.jpg">
    - One appropriate piece of documentation with this program would be a dedicated answer key manual where each image of the binary hand symbol is next to the bit representation and the number the hand represents in a table format with three columns (1 for image of symbol, 1 for bit representation, and 1 for number) and 33 rows (1 title row, 32 rows with 1 for each number from 0 to 31). This makes it easier to study the binary hand symbols and grade oneself + One appropriate piece of documentation would be a guide for how to translate the binary hand symbol into the number it represents, explaining how each finger represents a bit and each bit is 2^n with n = 0, 1, 2, 3, or 4 depending on the finger and then add up the sum of numbers each finger held up represents to get the overall number with examples.
    - This documentation would be used by aspiring coders who are trying to learn how binary counting works and to get familiar with its counting system and how bits can be used to represent numbers. They would read the documentation about how to translate hand symbol to number and then test themselves on what they just learned from the documentation using the quiz in the program. They can study the documentation to better deepen their understanding as well.

> Question 2:
- Component C: Personalized Project Reference <img src="https://i.postimg.cc/6QBkxdM4/Question2-Component-C.jpg">
    - Procedure
        - <img src="https://i.postimg.cc/J0sTVWGt/Answer4-Question1-Component-A.jpg">
        - <img src="https://i.postimg.cc/MTPsFGZh/Answer5-Question1-Component-A.jpg">
        - <img src="https://i.postimg.cc/J0BY9W2K/Answer1-Question2-Component-C.jpg">
    - List
        - <img src="https://i.postimg.cc/WbJ95jBH/Answer6-Question1-Component-A.jpg">
        - <img src="https://i.postimg.cc/7P2kvv7p/Answer2-Question2-Component-C.jpg">
- Question <img src="https://i.postimg.cc/Dw3VBVsg/Question2-Question.jpg">
    - a. There is no iteration used in the procedure section.
    - b. checkQuiz() would call the procedure, but the procedure takes no parameters so there are no arguments within the call. This call would run the procedure to check the answers in the quiz and output the number of correct and wrong answers, letting the user know if they answered correctly or not and potentially getting them to redo the quiz if they got some questions wrong.
    - c. If the list was gone, I would set each image link as its separate variable (for example, var image0 = (insert link corresponding to the binary hand symbol for 0) and so on for all 32 images). Then I would keep the Math.floor(Math.random()*32) to get a random number from 0 to 31 and set another variable where it concatenates that number at the end of the string "image", and that variable will be used as the image link in the .html.

## Planning for CPT Project
> General Notes for Project
- Final decision on project: Turn-based Fantasy Tarkov-esque game
- Various stats of characters or like equipment that increases stats
- Map with set location, can pick where to go + images for places and/or bosses/enemies/player
- Get a warning when people are near (maybe add sound)
- Can choose to like move out, attack, defend, etc.
- If attack someone, has % chance to defeat them
- No actual weapons, use either medieval weapons or like magic and classes
- If defeated, leave and back to start
- Can have like multiplayer or boss

> Question 1:
- Component A:
    - Parts missed
        - Procedures have no parameters
        - Procedures have no iteration
    - Include in CPT project
        - Keep having user input, this will be done in many ways including the JWT login authentication, the user selecting classes and creating their character, the user selecting actions to take in the game, etc.
        - Keep using lists, perhaps have a list for inventory and character information
        - ADD PROCEDURE WITH PARAMETERS AND ITERATION. Parameters can be used in procedures that calculate damage and health deduction and the paramters can be like currenthealth and resistance. Iteration can be to clean up repetitive code when it pops up, maybe when updating data to the data table or outputting character stats?
            - Procedure will need to be called so that's not an issue, but it needs to have arguments in the call
        - Keep having output, perhaps after each turn output remaining HP, enemy HP, information about attacks and actions to take, etc.
- Component B:
    - Parts missed
        - Nothing really missed
    - Include in CPT project
        - Record a short video showcasing the project working, just screenrecord it with windows key + g and then add captions using ClipChamp. Remember it's less than 1 minute long.
- Component C:
    - Parts missed
        - Procedure doesn't have return which isn't necessary, but it would be good to add and it can be implemented with the procedure calculating damage (return the deducted health or health after the calculations).
        - Procedure doesn't have parameters or iteration, see Component A.
    - Include in CPT project
        - Procedure with parameters or iteration, see Component A.
        - List is present and fulfills the requirements, so keep the list and remember to update data (probably will do this when creating/updating character, maybe have a stat upgrade system with objects found?)
- Question:
    - Would be cool to include some documentation with this program like a ReadMe, Guide/Tips/Strategies, How-To-Play, etc.
    - Not sure if this is 100% needed, but good to add

> Question 2:
- a. 
    - Parts missed
        - The CPT project NEEDS NEEDS NEEDS a procedure that will use iteration, so take any repetitive code and try to make it more concise with for/while loops.
    - Include in CPT project
        - Maybe add a button that outputs the users character stats and a loop can be used to do get requests from backend? Can try to do this with other requests like post. Think more about this with group.
- b. 
    - Parts missed
        - The CPT project NEEDS NEEDS NEEDS parameters to take in and calls with arguments.
    - Include in CPT project
        - Likely need a procedure that calculates damage done and remaining health, so will have parameters there (currenthealth, resistance, anything that boosts/change damage dealt like attack or weapon).
        - Ensure that it can be tested, and it probably will since you can use dummy numbers as the argument to test the math and output.
- c.
    - Remember to include list, see Q1 Component A and C. Think about alternate ways to make program work even if less efficient.