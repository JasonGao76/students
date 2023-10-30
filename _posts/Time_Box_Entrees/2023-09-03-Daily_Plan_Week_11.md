---
toc: true
comments: false
layout: post
title: Daily Plan Week 11
description: Daily plan for week 11
type: plans
courses: { compsci: {week: 11} }
---

## Monday:
> Work on API and data model, update with Matthew's CORS and remove inventory (implement and fix later)

> Update frontend repository

> Test GET, POST, PUT, DELETE and all works so qualify tomorrow

> Temporary: Syntax for get, post, put, delete requests
get:
send to http://localhost:5001/soulsCharacterList for character dataset, http://localhost:5001/soulsList?id=(id number) to get a specific class (ex: http://localhost:5001/soulsList?id=1 for God class) 
<br>
post:
{
    "id": id number,
    "name": "(name)",
    "gender": "(gender)",
    "age": number,
    "class_name": "(Class name)",
    "health": value
    "attack": value
    "resistance": value
    "power": value
}
ex:
{
    "id": 2,
    "name": "EEEEE II",
    "gender": "female",
    "age": 21,
    "class_name": "Warrior",
    "health": 110,
    "attack": 130,
    "resistance": 110,
    "power": 3
}
<br>
put:
{
    "id": id number,
    "(what you want to change)": (new value or string)
}
ex:
{
    "id": 1,
    "name": "EEEEE II"
}
<br>
delete:
{
    "id": id number
}

## Tuesday:
> 

## Wednesday:
> 

## Thursday:
> 

## Friday:
> 
