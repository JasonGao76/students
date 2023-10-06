---
toc: true
comments: true
layout: post
title: Passion Project Plan
description: Plan for our Passion Project
type: tangibles
courses: { compsci: {week: 7} }
---
## Plan for Passion Project
> Theme: Dark Souls or Terminal Souls
- Initially, we wanted to create a terminal game. We wanted to add areas from a Dark Souls game, cd into various areas to find objects, complete a puzzle, then add a turn-based game. However, we realized that this was quite ambitious, so we decided to focus on one part of that: the boss fight. Our idea is to have a turn based boss fight with various images, attacks, HP bars, and more.

> Roles
- Arthur: Backend
- Rayane: Frontend
- Isabelle: Frontend
- Matthew: DevOPS/Backend
- Me: DevOPS/Backend

> General Plan: Turn-Based boss fight, you click button --> image of boss is changed, your attack and power is grabbed from the backend and subtracted from the boss HP bar, update boss HP bar, boss hits you so get boss data and update your HP bar --> repeat

> Frontend
- Need to display text, HP bar, image of boss, and buttons for attacks
- Have it so every time after a button is pressed, change the image of the boss, HP bar, and maybe the text?

> Backend
- Include data sets of classes with HP, resistance, attack, and power (scale factor for attack)
- Include data set for boss
- Get REST API (get, post, delete), likely need lots of get for frontend to grab data from data set