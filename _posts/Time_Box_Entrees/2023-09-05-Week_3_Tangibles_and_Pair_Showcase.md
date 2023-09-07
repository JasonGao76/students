---
toc: true
comments: true
layout: post
title: Week 3 Tangibles, Plan for Pair Showcase, and Review Ticket
description: Summary and tangibles of what was done in week 3, the plan for the pair showcase, and the review ticket
type: tangibles
courses: { compsci: {week: 3} }
---
## Plan for Pair Showcase
- Plan is this page. GitHub Issues tracks what we have been working on: should have calculator, updating time box, linux, chatgpt, theme
- Ask teacher questions/collaboration: Ask about whether or not os.system (running Linux commands in Python) counts as linux and interaction in VSCode (DONE) + ask other groups questions about organizing and themes
- Linux: incorporate os.system in python to run linux commands, especially pip install
- Python: Python hacks (mean calculator/emoji/wikipedia), Python quiz
- JavaScripts: JS Calculator (mention challenges), JS Tables w/ jquery
- Update Time Box page and update as go along
- Review with ChatGPT: Used to help understand JS Calculator and help add sqrt function, summarize response and add ss
- Make review ticket below this and expand

## Review Ticket
> Plan: See above.

> GitHub Issues: Click <a href="https://github.com/JasonGao76/students/issues" target="_blank">here</a> to see GitHub Issues.

> Teacher Interaction: There were numerous interactions with the teachers, but the ones listed are the most relevant and important.
- Towards the beginning, our "make" command worked but the page was not found. After trying to fix the issue and failing, we asked Mr. Mortenson about how to fix it, and we were told to change "0.0.0.0:" to "localhost:", and it worked and allowed our blog to finally run properly.
- Through the blog check, we learned that our Time Box was not done correctly, so we took a look at the examples and other people's code to see what it was supposed to look like. After properly figuring out how to use front matter, we remade our table, updated all the pages, and tested it to make sure it worked.
- We had a plan to incorporate Linux commands into Python and combine multiple hacks into one, but we were not sure if it counted as the separate hacks. During Office Hours, I asked Mr. Mortenson whether or not it would count, and he said it would count because he mainly is trying to see whether or not we understand and can use the parts. Afterwards, we discussed whether or not the plans needed updating and what else we can add onto our hacks.
- The theme of our page was ruining the display of our code, so we asked Mr. Mortenson if it was ok to change the theme beforehand to let him know that we still attempted customization but we need to change it back to see the code. He said yes, seeing the progress is more important than how the blog looks in the showcase.

> Linux and VSCode
- Linux combined with Python_Hacks.

> Python and VSCode
- See Python_Hacks in the hacks column in the Time Box, or use Jupyter Notebooks.
- See Python Quiz in the hacks column in the Time Box, or use Jupyter Notebooks.

> Web interaction in JavaScript
- See JS Tables in the hacks column in the Time Box.
- See JS Calculator in Week 2 Tangibles in Time Box.

> All updated in Time Box page: 
- Check out the Time Box table in compsciTeacher!

> ChatGPT: We asked ChatGPT to help us explain the JavaScript in the JS Calculator. First we asked for a quick summary, then for help to add a square root function:
- Summary of code: ChatGPT told us that the code uses HTML, CSS, and JS to make a calculator with GUI and Vanta.js animation. The HTML markup creates a container div (id "animation") to hold calculator and animations, and has a calculator-container div in the container to hold the calculator elements. The CSS defines styles, and the main styles are making the .calculator-output class take up the first row of the calculator, have rounded corners, have a border and padding, and have a font size, and the .row class to have rows. The JS adds functionality by defining firstNumber/operator/nextReady, selects DOM elements using document.getElementById and document.querySelectorAll, has event listeners that detect when these buttons are clicked, and defines functions for numeric, opration, calculate, equal, and clearCalc buttons. Lastly, the code includes Vanta.js animations and imports various scripts to set up random animations.
- Add square root function: Add new div element with calculator-operation class (kinda sketchy because the other operations are defined with first and second but sqrt doesn't have second), create event listener for square root button, add new function to calculate square root, and modify operation and calculate function. This did not really work in the end, partially because we did not fully understand the JavaScript behind the calculator or the ChatGPT code and also because the ChatGPT code did not really take into consideration the other code and the arguments "first" and "second" for the operation functions.
- The div element: &nbsp; <img src="https://media.discordapp.net/attachments/1143438030749847604/1148881519570604132/image.png">
- The modifications to JS: <img src="https://media.discordapp.net/attachments/1143438030749847604/1148881587140833310/image.png">
<img src="https://media.discordapp.net/attachments/1143438030749847604/1148881626026225684/image.png">

> Review Ticket:
- This page right now!


## Summary and Accomplishments
- Updating blog
- Python_Hacks (mean calculator, emojis, import libraries, Linux)
- JS Output tables with jquery
- JS Calculator
- Review Ticket
- Pair Showcase