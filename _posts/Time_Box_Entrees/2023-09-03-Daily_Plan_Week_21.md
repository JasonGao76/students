---
toc: true
comments: false
layout: post
title: Daily Plan Week 21
description: Daily plan for week 21
type: plans
courses: { compsci: {week: 21} }
---

## Monday:
> Spot check
- Database with database change
    - Schema change, work with columns not rows
    - Developer do in backend and code in frontend to access, not frontend can modify it
    - To activate, delete current database and run migrate.sh again
- Postman with /authentication screen
    - Authenticate through postman and have authentication screen, includes authentication through website
- Postman with /api screen to access data under authentication
    - Be able to read and display user database on website
- Jupyter notebook or web page that shows signup and login
    - Aim for webpage, no jupyter is ok + show you can sign up a user and login
- Jupyter notebook or web page that shows redirect of 403 to signup and login page
    - 403 is unauthorized, no permissions + make html for 403 to show
- Jupyter notebook that shows CRUD operation on page that requires authentication
    - Create, read, update and delete + @token_required

> Work on spot check and individual JWT

## Tuesday:
> Worked on spot check and individual JWT

## Wednesday:
> CPT Spot check, didn't get to go so spent time polishing it up

## Thursday:
> Student teach; SASS / Javascript Login and Signup Page
- SASS has nesting, variables, etc.
- Frontend can give error status code like 403
- Response code - Send request to backend, can get different response codes depending on what happens, 200 is success --> 403 is no authentication, 404 is page doesn't exist
- Common HTML stuff includes input fields (can set type to password), containers to group elements, and common properties include buttons, placeholders, class
- Hack 1: SASS is extension of CSS
- Hack 2: Lower one has SASS, top has no SASS
- Hack 3: If get 403, means no authentication and should try logging in or getting cookie
- 401 is never authenticated whatever, 403 is user but try to access smth only admins can access
- To create database
    - Get user info, make frontend, make backend handling, make api
- GET method to get authentication before showing page and add error handling

> When making new column, delete all backups and copies of database then run migrate.sh and make sure table view is set to users or whatever you're trying to look at

> Did CPT Spot check, got 0.92 for first point and 0.91 for second and third point
- Since >0.9 for all three, counts as 2/2

## Friday:
> Continue working on individual JWT
