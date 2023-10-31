---
toc: true
comments: true
layout: post
title: Reference for PP Request Syntax
description: Has references and/or examples for each type of request (GET, POST, PUT, DELTE) that can be used for our Passion Project Terminal Souls
courses: { compsci: {week: 11} }
type: hacks
---

# GET
## Fetch/See data from data table
URL to send to: <br>
http://localhost:5001/soulsCharacterList for character dataset <br>
http://localhost:5001/soulsList?id=(id number) to get a specific class <br>
Example: http://localhost:5001/soulsList?id=1 (to get God class)

# POST
## Post/Add a new entry into data table
General syntax (REMEMBER TO GO TO Body --> raw --> change Text to JSON): <br> <!-- without the <br> and &nbsp; -->
{ <br> 
&nbsp;&nbsp;&nbsp;&nbsp;"id": id number, <br> <!-- id number should be the one corresponding to the class -->
&nbsp;&nbsp;&nbsp;&nbsp;"name": "(name)", <br>
&nbsp;&nbsp;&nbsp;&nbsp;"gender": "(gender)", <br>
&nbsp;&nbsp;&nbsp;&nbsp;"age": number, <br>
&nbsp;&nbsp;&nbsp;&nbsp;"class_name": "(Class name)", <br>
&nbsp;&nbsp;&nbsp;&nbsp;"health": value <br>
&nbsp;&nbsp;&nbsp;&nbsp;"attack": value <br>
&nbsp;&nbsp;&nbsp;&nbsp;"resistance": value <br>
&nbsp;&nbsp;&nbsp;&nbsp;"power": value <br>
} <br> <br>
Example: <br>
{ <br>
&nbsp;&nbsp;&nbsp;&nbsp;"id": 2, <br> 
&nbsp;&nbsp;&nbsp;&nbsp;"name": "EEEEE II", <br>
&nbsp;&nbsp;&nbsp;&nbsp;"gender": "female", <br>
&nbsp;&nbsp;&nbsp;&nbsp;"age": 21, <br>
&nbsp;&nbsp;&nbsp;&nbsp;"class_name": "Warrior", <br>
&nbsp;&nbsp;&nbsp;&nbsp;"health": 110, <br>
&nbsp;&nbsp;&nbsp;&nbsp;"attack": 130, <br>
&nbsp;&nbsp;&nbsp;&nbsp;"resistance": 110, <br>
&nbsp;&nbsp;&nbsp;&nbsp;"power": 3 <br>
}

# PUT
## Put/Update data in data table
General syntax (REMEMBER TO GO TO Body --> raw --> change Text to JSON): <br>  <!-- without the <br> and &nbsp; -->
{ <br>
&nbsp;&nbsp;&nbsp;&nbsp;"id": id number, <br> <!-- id number should correspond to the entry in the soulsCharacter data table, NOT the class -->
&nbsp;&nbsp;&nbsp;&nbsp;"(what you want to change)": (new value or string) <br>
} <br> <br>
Example: <br>
{ <br>
&nbsp;&nbsp;&nbsp;&nbsp;"id": 1, <br>
&nbsp;&nbsp;&nbsp;&nbsp;"name": "EEEEE II" <br>
}

# DELETE
## Delete/Remove data from data table
General syntax (REMEMBER TO GO TO Body --> raw --> change Text to JSON): <br> <!-- without the <br> and &nbsp; -->
{ <br> 
&nbsp;&nbsp;&nbsp;&nbsp;"id": id number <br> <!-- id number should correspond to the entry in the soulsCharacter data table, NOT the class -->
} <br> <br>
Example: <br>
{ <br>
&nbsp;&nbsp;&nbsp;&nbsp;"id": 1 <br>
} <br>