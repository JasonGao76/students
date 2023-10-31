---
toc: true
comments: true
layout: post
title: Individual Project Final
description: Review ticket, or plan, for what to cover in the Final Project - Individual check. Covers both the individual code and the individual blog, but more in-depth information about the individual code are on te GitHub Issues linked.
type: tangibles
courses: { compsci: {week: 11} }
---
## Individual Code
> Please see the GitHub Issues named "modules and import data not working + get user input for class", "New API and Model to handle Player, Update Model and try to post a List", and "Error Maximum Recursion Depth Exceeded" on repository JARMIRAMJI for what I mainly worked on.
- ["Modules and import data not working + get user input for class"](https://github.com/dino596/JARMIRAMJI/issues/2): This was the first issue and big thing that we as backend tracked. This was after the Flask server was up and running and we had already tried making an API (with all the functions defined) but there were a few errors. This logged the issue we had (attribute and name errors) and gave more information and potential solutions. Then after we fixed it by correcting the modules imported, we updated the issue with what was wrong and how we fixed it. Then we included what we were doing after that, which was trying to incorporate user input with class and planning how to get it to work with frontend, then experimenting with finding a way to send the whole data set over. This GitHub Issue was left there because after this, we discovered SQAlchemy and experimented with that and found that it was much more efficient than what we were currently doing, presented the data in a nicer way, and was better suited for the needs of our project, so we swapped to that and this issue didn't apply to that anymore. Personally, I was the one who tracked this issue with the requests, elaborated on the error and potential fixes, and eventually did fix it by correcting the imports.
- ["New API and Model to handle Player, Update Model and try to post a List"](https://github.com/dino596/JARMIRAMJI/issues/3): First off, this tracked the progress backend has completed with the new API and data model needed to handle a separate "player" class the frontend wanted. This had to be separate from the original data model with the class data since frontend wanted to add unique information (such as name, gender, age, etc.) that the other classes did not. So, we created this API and data model by essentially taking our one we made for the preset classes is the issue above, then altering it to fit this purpose. We had to alter the names and thus the imports, add arguments to add for the new entry, establish new endpoints, and run and debug as usual. Personally, I was the one who worked on the data model, so I was the one tweaking which new pieces of information were going to be initialized and accepted into the data model, the data types it would allow, and setting new properties. I also experimented with how the player data model would be initialized and communicated with frontend, since I could either just have a completely empty data model OR have placeholder values. We decided that there wouldn't be any difference since frontend would POST new data and override it anyways, so a completely empty data set can potentially avoid any issues with the request. Later, when also communicating with frontend, they told us that they wanted an inventory property for the player as well. So I worked on adding the new value into the data model and found something to potentially work on. This and everything else is explained more in detail in the actual issue, but a quick summary is that the API can handle a list (instead of string) but the data model can't. This isn't program-breaking but would make the data look neater and make frontend's job easier and is something to keep looking into.
- ["Error Maximum Recursion Depth Exceeded"](https://github.com/dino596/JARMIRAMJI/issues/4): Issue where we got the error "Maximum Recursion Depth Exceeded", which was completely new. This occurred with the PUT request if multiple values in the data table are updated in the same request. This isn't program-breaking since multiple PUT requests can be sent, each changing one thing, but fixing this error would make the frontend's job much easier. This is here to track progress and prove that these projects will always be continuously developed, tested, and improved upon. The issue has more in depth information about the error, screenshots, and potential ways to fix. I was the one who found the error, tracked and logged it, and proposed potential fixes.

> GitHub Analytics: I have been continuously working and committing, as proven by having commits for most days and definitely multiple per week. [Here is my GitHub profile!](https://github.com/JasonGao76)

> Key GitHub commits: 
- [10/3 passionproject update](https://github.com/dino596/JARMIRAMJI/commit/f57832e8aa83ec78d95264189d3d4e722fdcb13a): Created all the preset class data sets in the data model to send requests to.
- [10/13 updates](https://github.com/dino596/JARMIRAMJI/commit/05e0d86af08da394a1451f01ab90d8f7e1d04936): Corresponds to ["Modules and import data not working + get user input for class"](https://github.com/dino596/JARMIRAMJI/issues/2) issue where I fixed and experimented with the imports and changed the GET request to actually work and request a specific class data.
- [10/24 added soulsCharacter model](https://github.com/dino596/JARMIRAMJI/commit/954c2b3674364741816ddafe1a0ff8209700e503): Corresponds to ["New API and Model to handle Player, Update Model and try to post a List"](https://github.com/dino596/JARMIRAMJI/issues/3) issue, added the new data model for the player class and did some minor edits to the API to correctly call the soulsCharacter data model not the souls datamodel.

## Individual Blog
> Code in blog
- Student Lessons (see right in explorer in VSCode) name all changed to include "SL" in the beginning to indicate that they are student lessons. All of them are also on the TimeBox.
- All hacks and questions completed. The homework questions I am most proud of are Iteration extra credit, list and search binary search question, and list and search extra credit.

> Usage of blog
- See TimeBox! Everything has been continuously logged with daily plans and hacks. A big use of this blog was for student lessons as you can see from the hacks, and the key student lessons that I thought were personally the most helpful are marked with an asterisk.
- Part of the Passion Project was also included onto the blog by adding a reference for the various syntaxes for the different requests we can send to the data model.

> Psuedo-code notes
- Uses "<--" instead of "="
- Has "MISSING CODE" within <> to denote missing code
- Uses "IF" (or "IF ()"), "ELSE", "OR", etc. in all caps + no elif equivalent
- Has indents to indicate what code is within what statement/condition like Python but no ":", and also uses different shading to indicate it as well
- Uses "REPEAT (insert number) TIMES" (or "REPEAT UNTIL (condition)") and "{ (code) }" instead of while or for loops + or has "REPEAT UNTIL (variable) > (number)"
- Has "RANDOM x, y" to pick a random number between x and y instead of importing a library and "random.randint(x,y)"
- For functions/procedures, uses "RETURN" in all caps
- Uses "DISPLAY (insert what to display)" instead of "print(insert what to display)"
- Uses "PROCEDURE __ ()" instead of "def __()" and "{}" instead of ":"
- Robot commands: CAN_MOVE (left/right/forward/backward), ROTATE_RIGHT(), ROTATE_LEFT(), MOVE_FORWARD(), MOVE_BACKWARD(), GoalReached
- Uses "INPUT ()" in all caps
- 

> Collegeboard Quiz notes
- Question 3: Citizen science?
- Question 6: Internet Engineering Task Force?
- Question 12-13, 32: Shows data and need to interpret trends, can use logic
- Question 15: Asks about the Internet, can use logic
- Question 8, 16: Has a user do something and asks about what data can be found, what consequences, 
- Question 17: Digital divide = gap in technology?
- Question 21, 26, 31: Robot question
- Question 23: Redundant routing?
- Question 24: lossy vs. lossless, review this more
- Question 33: flowchart
- 

> Trimester 1 reflection
- Looking back at my Timebox, there were many great memories in this class. In the beginning, the Python Quiz and the Python Hacks really stood out to me. When I entered this class, I only really knew how to code a little in Python and walked in with the goal of expanding my ability to code in Python, so these two assignments really gave me what I was looking for and gave me opportunities to further explore what Python can do. I remember spending a ton of time on especially the Python Hacks to make it fun and personal, all the while learning about how to use libraries, logically set variables and do mathematical operations with them, set logical conditional statements, get used to the syntax, and so much more. The Python Hacks assignment was one of the first assignments I was quite proud of myself in doing. Next, I thought that the Web Programming test was definitely unique and deserved a mention. It was a LOT of work to complete and I remember pouring hours into not only completing it, but getting each section to be personal and outputted correctly (it also didn't help that VSCode for me kept crashing for me here for some reason). It was also one of my first experiences with Javascript, which definitely broadened my horizons and made me look at what other code languages offered. Something I want to work on in future trimesters is to continue practicing with Javascript and maybe make a separate project if I have the time. I would also like to continue learning more about Python, since even though I did learn a lot this trimester, there is so much more to do, and one example is learning in-depth about the classes and how they work. The API and Passion Project did expose me to these concepts and forced me to somewhat learn them, but I would love to learn them properly in the classroom as well. The Passion Project was and is my most favorite thing we have done this trimester. It really allowed for creativity in what to do, incorporated multiple coding languages, and pushed us to learn things on our own and develop our own methodology of working. While sometimes it was painful and took way more time than it should have, I definitely learned a lot from it. AND I met Rayane :D. Lastly, the Student Lessons definitely helped me with solidifying the fundamentals. Again, I entered this class with virtually no previous experience, so these lessons were very useful in getting the basics down and practicing what I already know and learned. It also really pushed us to learn more about Collegeboard's pseudo-code and how Collegeboard likes to ask questions, so this definitely helps with knowing what to expect from the AP exam. I also got to connect more with the other students, and teaching the lesson was pretty fun! Throughout the whole trimester, I was working closely with my partner Arthur, and it was very interesting to talk to him about what we were working on (especially since he knows more than I do when it comes to code) and fun to bond over the common issues we faced. I definitely got to know him better this trimester and I hope we have the same CSP period next trimester as well! Overall, a great trimester with many wonderful memories, but I would love to continue deepening my knowledge about Python and getting more familiar with Javascript (and pseudo-code).