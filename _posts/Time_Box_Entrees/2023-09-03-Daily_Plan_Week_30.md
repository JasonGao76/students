---
toc: true
comments: false
layout: post
title: Daily Plan Week 30
description: Daily plan for week 30
type: plans
courses: { compsci: {week: 30} }
---

## Monday:
> Presented Data Structure Cross-over to Mr. Lopez, not for a grade and just show that I did it

> Start polishing CPT for AP Exam

## Tuesday:
> Deployment lecture
- Use config.js to reduce repeated code
- Nginx helps direct requests to the right server
- Docker is on localhost, nginx is not
- Access-Control-Allow-Origin controls what link / domain is allowed to access / send a request to the server
- Access-Control-Allow-Methods controls what requests are allowed to be made
- @token_required in places where authorization is meant to be
- Update init.py to have frontend website
- SECRET_KEY to have security for website and help stop cross-origin attacks
- Certbot gives website a certificate, allowing it to use HTTPS (HTTPS has security, HTTP does not) so it's trusted and communications are secure
- Internet breaks data down into packets and sends these small packets to wherever it needs to go
    - Internet is inherently fault tolerant due to multiple connections to nearly every place
- All related to networking
- Parallel/distributed computing is having multiple systems all do the same task at the same time, and it also provides fault tolerance because another system can pick up the job that another one failed at
- Gunicorn is Python for web server, and can set how many instances of server to run (provides fault tolerance in case one crashes/fails)
    - --workers=1, means 1 instance

> Continue polishing CPT for AP Exam
- Can add more features: enemy attack only if it can hit you (done), actually make range/movement work, polish up comments and console.log
- Prepare for CPT submission and do Collegeboard written examination practice

## Wednesday:
> Continue polishing CPT and fixing it / adding features
- Frontend should be all good (unless want to add range/movement functionality)
- Backend, currently working on classes.py (model)

## Thursday:
> 

## Friday:
> 