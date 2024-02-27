---
layout: post
title: Individual Final
hide: true
comments: true
description: Individual final for CPT Project and CSP Final, correlation to CPT showing how my features/pull requests map to CollegeBoard requirements
type: tangibles
courses: { compsci: {week: 23} }
---

# Personalized Project Reference
> Procedure: Capture and paste two program code segments you developed during the administration of this task that contain a student-developed procedure that implements an algorithm used in your program and a call to that procedure.
- i. The first-program code segment must be a student-developed procedure that:
    - Defines the procedure's name and return type (if necessary)
    - Contains and uses one or more parameters that have an effect on the functionality of the procedure
    - Implements an algorithm that includes sequencing, selection and iteration
- ii. The second program code segment must show where your student-developed procedure is being called in your program.

> Procedure answer
- The procedure's definition: ("https://i.postimg.cc/hjXggxN5/Procedure-1.png")
- The procedure's call: <a href = "https://i.postimg.cc/0QhvNjs2/Procedure-2.png">
- The HTML the procedure is referring: <a href = "https://i.postimg.cc/02RxRznV/Procedure-3.png">

> List/Collection: Capture and paste two program code segments you developed during the administration of this task that contain a list (or other collection type) being used to manage complexity in your program.
- i. The first program code segment must show how data have been stored in the list.
- ii. The second program code segment must show the data in the same list being used, such as creating new data from the existing data or accessing multiple elements in the list, as part of fulfilling the program's purpose.

> List/Collection answer
- The collection's definition: <a href = "https://i.postimg.cc/GtYCTRLP/Collection-1.png">
- The collection being used: <a href = "https://i.postimg.cc/J7Bm2NNy/Collection-2.png">

# CollegeBoard Requirements

## Component A: Program Code

### Purpose of the Program
- The purpose of my program/game is to provide entertainment to the user while also strengthening their logical thinking and reasoning by having them predict where the AI could be in order to maximize their probability of winning.

### Instructions for input from one of the following: the user, a device, an online datas stream, a file.
- The program takes input from the user through the movement/attack input boxes, and the value of the number inputted is saved and used to determine where to move the user or where to attack.
- Using the procedure as a reference: the arguments to the procedure call are the variables "position", which is a number, and enemyspot, which is an "array", and the procedure checks if the number is a number in the array.

### Use of at least one list (or other collection type) to represent a collection of data that is stored and used to manage program complexity and help fulfill the program’s purpose.
- The collection: <a href = "https://i.postimg.cc/GtYCTRLP/Collection-1.png">
- possibleActionPositions is defined as an object with multiple key-value pairs where the key is the number corresponding to each position on the map and the value is a list of numbers corresponding to the positions the position of the key can act (move/attack) on.

### At least one procedure that contributes to the program’s intended purpose, where you have defined: the procedure’s name, the return type (if necessary), one or more parameters
- The procedure: <a href = "https://i.postimg.cc/hjXggxN5/Procedure-1.png">
- Name: checkPosition
- Return type: Boolean "true"
- Parameters: "number" (integer) and "arr" (array)

### An algorithm that includes sequencing, selection, and iteration that is in the body of the selected procedure
- The procedure also fulfills this requirement: <a href = "https://i.postimg.cc/hjXggxN5/Procedure-1.png">
- The algorithm iterates through each number in the array and checks if it is equal to the number argument passed through the call

### Calls to your student-developed procedure
- The call: <a href = "https://i.postimg.cc/0QhvNjs2/Procedure-2.png">
- checkPositions is called two ways: first is where a variable "check" is defined as the returned value (true) of checkPosition and second is where checkPosition is simply run to ensure that the HTML text changed. In both situations, the variable "position" is passed as the argument for the parameter of "number" and the array "enemyspot" is passed as the argument for the parameter of "arr"

### Instructions for output (tactile, audible, visual, or textual) based on input and program functionality
- The procedure: <a href = "https://i.postimg.cc/hjXggxN5/Procedure-1.png">
- The HTML referenced: <a href = "https://i.postimg.cc/02RxRznV/Procedure-3.png">
- The HTML defines multiple spans using id, and the procedure gets these spans using getElementById and uses .textContent to update the text in the spans, creating a textual output.

## Component B: Video
### Link
- [Link to video](https://drive.google.com/file/d/1ED5nYx31NEW3jXDGaeo-fYEcrK7elP10/view?usp=sharing)

### Input to your program
- Has user input numbers of the positions to move to

### At least one aspect of the functionality of your program
- Showcases the movement aspect of the program/game's functionality

### Output produced by your program
- Shows the text output and image changes of the program

### Your video may NOT contain: Any distinguishing information about yourself; Voice narration (though text captions are encouraged)
- There is no information about myself in the video
- There is no voice narration, and there are text captions

### Your video must be: Either .webm, .mp4, .wmv, .avi, or .mov format; No more than 1 minute in length; No more than 30MB in file size
- The video is .mp4
- The video is 1 minute long
- the video is 10.8 MB