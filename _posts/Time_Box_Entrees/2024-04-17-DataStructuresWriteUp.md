---
layout: post
title: Data Structures Write Up
hide: true
comments: true
description: 
type: tangibles
courses: { compsci: {week: 29} }
---

> Collections
- Blog Python Model code and SQLite Database.
    - From VSCode using SQLite3 Editor, show your unique collection/table in database, display rows and columns in the table of the SQLite database.
        - <img src="https://i.postimg.cc/mD1zwY7g/Collections-1.png">
            - This is the database used in our data structures project to save the inputs of the user. It has id, socialclass, age, sex, siblings, family, fare, port, and alone as the unique columns, and each row is a new entry / submission (after being processed) from the user.
        - From CPT: <img src="https://i.postimg.cc/yY5GcYLy/Collections-CPT-1.png">
            - This is the database used in our CPT project to define the preset classes the user can choose from. It has id, classname, health, attack, range, and movement as the unique columns, and each row is a preset class the user can choose from to make their character and play the game with. The data of the class the user chooses is retrieved from this database and saved in a separate datatable so it can be updated as the user plays the game.
    - From VSCode model, show your unique code that was created to initialize table and create test data.
        - <img src="https://i.postimg.cc/PrQL2rvY/Collections-2.png"><img src="https://i.postimg.cc/MKSM7jHz/Collections-3.png"><img src="https://i.postimg.cc/3rp00ZKL/Collections-4.png">
            - The datatable used in the data structures project is defined under class DS, and within it the table is named, the arguments are made, init is defined, each argument is made into a property and is set, and the table is initialized.
        - From CPT: <img src="https://i.postimg.cc/ZRTs49q4/Collections-CPT-2.png"><img src="https://i.postimg.cc/3wQbff5y/Collections-CPT-3.png"><img src="https://i.postimg.cc/zDx6DkWM/Collections-CPT-4.png"><img src="https://i.postimg.cc/Gmy5QwNw/Collections-CPT-5.png">
            - The datatable used in the CPT Project is defined under class Classes, and within it the table is named, the arguments are made, init is defined, each argument is made into a propert and is set, and the table is initialized while also defining and adding the preset class data to the table.

> Lists and Dictionaries
- Blog Python API code and use of List and Dictionaries.
    - In VSCode using Debugger, show a list as extracted from database as Python objects.
        - Dictionary with a list in it, so this is also for the question below: <img src="https://i.postimg.cc/DZG0s2KW/List-Dictionary-1.png"><img src="https://i.postimg.cc/wMdvQS6w/List-Dictionary-2.png">
            - Passenger is the dictionary (also for the second question), and within it has lists for columns and the axes for the Titanic ML.
        - From CPT: <img src="https://i.postimg.cc/4NnMYhQ3/List-Dictionaries-CPT-1.png">
            - CurrentCharacter uses a list of the classes to get a specific class and then make that the currentcharacter.
    - In VSCode use Debugger and list, show two distinct example examples of dictionaries, show Keys/Values using debugger.
        - <img src="https://i.postimg.cc/5yqt7nyb/List-Dictionary-3.png"><img src="https://i.postimg.cc/v8WDZHzk/List-Dictionary-4.png"><img src="https://i.postimg.cc/m2BkzfpD/List-Dictionary-5.png"><img src="https://i.postimg.cc/Wb830Wx7/List-Dictionary-6.png"><img src="https://i.postimg.cc/ht3t5JDz/List-Dictionary-7.png">
            - Titanic_data is a dictionary used by the Titanic ML and includes the various inputs for the ML, including age, alone, embarked, and so on.

> APIs and JSON
- Blog Python API code and use of Postman to request and respond with JSON.
    - In VSCode, show Python API code definition for request and response using GET, POST, UPDATE methods. Discuss algorithmic condition used to direct request to appropriate Python method based on request method.
        - GET
            - From CPT: <img src="https://i.postimg.cc/wxJbFxJq/APIJSONCPT-1.png">
                - GET used in CPT project GETS all the users from the database of current characters, iterates through it to a specific character, and returns that character in json format.
        - POST
            - <img src="https://i.postimg.cc/NMZTqJQX/APIJSON-1.png"><img src="https://i.postimg.cc/W1Skbb2T/APIJSON-2.png"><img src="https://i.postimg.cc/3J5ptcS5/APIJSON-3.png">
                - POST used by data structure Titanic ML to define arguments for each passenger, creates a new passenger to feed into the ML (and gets values from frontend), trains the ML with a logistical regression model to predict dead and alive probability (note that it's inefficient to train ML every time), and runs the ML using the passenger defined earlier to find and return the probability of surviving.
            - <img src="https://i.postimg.cc/BnJF01fm/APIJSON-4.png">
                - POST used by data structure Covid ML to define mock database, train ML with logistical regression model to predict risk level, calculates risk level by running ML using the data sent from the frontend, and returns risk.
        - UPDATE
            - From CPT: <img src="https://i.postimg.cc/m2ypfd8K/APIJSONCPT-2.png">
                - PUT used in CPT project gets the new character data from the frontend and creates a new character in the currentCharacter datatable, overriding the first row (index 0) with the new data. This works in the context of our game since the user only plays with one class at a time, but does offer a potential feature to have the user be able to save the data of the characters they play. This also somewhat acts as our DELETE as it overrides the old data with the new data, deleting the old data as a result.
    - In VSCode, show algorithmic conditions used to validate data on a POST condition.
        - <img src="https://i.postimg.cc/WzrZ2G4H/APIJSON-5.png">
            - Cleans and processes the inputted data to convert sex and age into binary true/false.
        - From CPT: <img src="https://i.postimg.cc/cLdjvqvs/APIJSONCPT-3.png">
            - Ensures data is correct and valid for the data the input is for.
    - In Postman, show URL request and Body requirements for GET, POST, and UPDATE methods.
        - GET
            - From CPT: <img src="https://i.postimg.cc/sgKLSnW5/APIJSONCPT-4.png">
                - Sent to currentchar to get the current character's stats.
        - POST
            - <img src="https://i.postimg.cc/yYmRtytJ/APIJSON-6.png">
                - Sent to Titanic api to calculate the survivability percent.
            - <img src="https://i.postimg.cc/xjbMy2P3/APIJSON-7.png">
                - Sent to Covid api to calculate the risk.
        - UPDATE
            - From CPT: <img src="https://i.postimg.cc/6Qm1byY3/APIJSONCPT-5.png">
                - Sent to currentchar to update current stats with new stats.
    - In Postman, show the JSON response data for 200 success conditions on GET, POST, and UPDATE methods.
        - GET
            - From CPT: <img src="https://i.postimg.cc/7hvtDjvr/APIJSONCPT-6.png">
                - Received the current character's statistics
        - POST
            - <img src="https://i.postimg.cc/FKRJf5Rc/APIJSON-8.png">
                - Received survivability probability (0.807)
            - <img src="https://i.postimg.cc/pd65zGhS/APIJSON-9.png">
                - Received risk (83.802)
        - UPDATE
            - From CPT: <img src="https://i.postimg.cc/c4SkzqMQ/APIJSONCPT-7.png">
                - Outputs the new stats.
    - In Postman, show the JSON response for error for 400 when missing body on a POST request.
        - <img src="https://i.postimg.cc/qqftZNGX/APIJSON-10.png">
            - No body in POST to get survivability probability, got 400 Bad Request error.
        - <img src="https://i.postimg.cc/HnQJGTZG/APIJSON-11.png">
            - No body in POST to get risk, got 400 Bad Request error.
    - In Postman, show the JSON response for error for 404 when providing an unknown user ID to a UPDATE request.
        - From CPT: N/A, our PUT was a little weird as we configured PUT to simply replace the first row in our liquid database with the new data in the body, allowing for a cleaner database.

> Frontend
- Blog JavaScript API fetch code and formatting code to display JSON.
    - In Chrome inspect, show response of JSON objects from fetch of GET, POST, and UPDATE methods.
        - GET
            - From CPT: <img src="https://i.postimg.cc/L84CHzW5/APIJSONCPT-8.png">
                - Data is the JSON object that was fetched and is the current character's stats (attack, classname, health, id, movement, range). Notice the current health of 10.
        - POST
            - <img src="https://i.postimg.cc/pLddCQHM/Frontend-1.png">
                - Response is the JSON object and has the information relevant to the fetch.
            - <img src="https://i.postimg.cc/cJgLysCD/Frontend-2.png">
                - Same as above.
        - UPDATE
            - From CPT: <img src="https://i.postimg.cc/HkSSjrG2/APIJSONCPT-9.png">
                - Data is the JSON object that was fetched and is the current character's stats (attack, classname, health, id, movement, range). Notice the new health of 11.
    - In the Chrome browser, show a demo (GET) of obtaining an Array of JSON objects that are formatted into the browsers screen.
        - In JavaScript code, describe fetch and method that obtained the Array of JSON objects.
            - From CPT: When the user is creating a character and selects a class, the frontend GETs that class's data and iterates through it and the hidden table to display the data in the browser.
        - In JavaScript code, show code that performs iteration and formatting of data into HTML.
            - From CPT: <img src="https://i.postimg.cc/G2TgWd5j/APIJSONCPT-10.png"><img src="https://i.postimg.cc/yxFQNnBg/APIJSONCPT-11.png">
                - Code iterates through the data of the selected class to add each stat into the table in the proper place to display it.
    - In the Chrome browser, show a demo (POST or UPDATE) gathering and sending input and receiving a response that show update. Repeat this demo showing both success and failure.
        - In JavaScript code, show and describe code that handles success. Describe how code shows success to the user in the Chrome Browser screen.
            - <img src="https://i.postimg.cc/7LffH3sn/Frontend-3.png">
                - Code updates the result and result2 span with hardcoded text and the return from POST respectively, showing the user that the request was successful. If the request wasn't successful, the result2 span wouldn't be updated with a number and display NaN instead.
            - <img src="https://i.postimg.cc/dVQhXPGX/Frontend-4.png">
                - Code updates the result3 span with the return from the second POST (and some additional hardcoded text), showing the user that the requestion was successful. Similarly to the explanation above, if the request wasn't successful, the result3 span wouldn't be updated properly.
        - In JavaScript code, show and describe code that handles failure. Describe how the code shows failure to the user in the Chrome Browser screen.
            - <img src="https://i.postimg.cc/6qQNNXfj/Frontend-5.png">
                - Code when receiving an error from the fetch first logs the error in console and then updates the result span with text notifying the user that there was an error and to check their inputs in the HTML, as that is likely the issue. The result2 span is left alone and stays empty (so nothing is displayed).
            - <img src="https://i.postimg.cc/1XY1mjW9/Frontend-6.png">
                - Code when receiving an error from the fetch first logs the error in console and then updates the result3 span with text notifying the user that there was an error and to check their inputs in the HTML, as that is likely the issue as if there was an error with the first POST above, this POST will also receive an error, meaning that an issue with the first POST (which is likely the user inputs) can also cause an issue with this POST.