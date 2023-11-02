---
toc: true
comments: true
layout: post
title: Outline for N@TM Presentation
description: Diagrams, plans, and notes for what to do at the N@TM Presentation to showcase our project
courses: { compsci: {week: 11} }
type: hacks
---

# Diagram
> <img src="https://media.discordapp.net/attachments/1143438030749847604/1169516682507714590/image.png?ex=6555b049&is=65433b49&hm=1b0928caa1c73e18193a078f275861eabe2f32e712d7e60ced220559a7adbdea&=">
- Here is a diagram of the interaction between two computers (frontend) and database (backend).
- The database stores the preset class stats (health, attack, resistance, power) and creates an empty "player" dataset. The frontend takes the user input on the character selection screen and when the user selects a class, the computer fetches the class data from the database using a GET request and displays it. When they enter their unique information about their character on the character selection screen (name, gender, and age) and pick a class, all that information is saved into the empty dataset on the local storage on the computer AND sent back to and saved in the backend through a POST request. After the player beats a boss and upgrades their player stats, the new information is updated in the computer's local storage AND updated in the backend dataset through a PUT request. 
- The reason all information is also stored in the backend is to give the leaderboard functionality beyond the local computer. The leaderboard is essentially all the data from the backend data model which houses every character created. Thus, when a computer locally creates a character and the data is sent to the backend, that character data is saved in the backend, so another computer seeing the leaderboard will GET the data from the backend and the new character will be displayed despite being created on a different computer.

# Plan
- First have two computers set up, one on the beginning screen before the title screen and another presenting the leaderboard.
- Then give a general explanation of what our project is: Our project is called Terminal Souls and it is a turn-based combat game that is themed around the Dark Souls franchise and modeled to be played in a linux terminal. 
- Then we will briefly explain the frontend and backend: The frontend is the screen you see here, the other screens you will see later, the leaderboard on the other computer, the animations and movement, and everything you can literally see on the screen. The backend comprises of the data, so the numbers and functionality of the game is done by the backend.
- Then the user will continue to create a character (where we will introduce the GET and POST requests), type commands in the terminal, and play the game. When they beat the boss, they will arrive at the upgrade screen (where we will introduce the PUT request). After upgrading their character, it will update on the leaderboard on the other computer and we will explain how that worked (the backend stores every character that has been created, and the data for the character made on the computer is sent to the backend. Since the leaderboard is a GET request to the backend and the data made on the first computer is sent and stored in the backend, the second computer can see the data made on the first computer).