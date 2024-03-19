---
layout: post
title: 2021 MCQ Reflection
hide: true
comments: true
description: 
type: tangibles
courses: { compsci: {week: 25} }
---

> Overview
- Score: 65/70
- Time: 58 minutes (class time) + 15 minutes (finish after school) = 73 minutes

> Reflection
- Questions I found difficult/didn't know much about beforehand
    - 9: [![JXOSTmJ.md.png](https://iili.io/JXOSTmJ.md.png)](https://freeimage.host/i/JXOSTmJ)
        - Use logic to do process of elimination, audio is usually measured in bits (bitrate and stuff like that) and it makes no sense for audio to be represented as procedures, operations to recreate sound, or text describing the sound.
    - 43: See below
    - 44: See below
    - 47: See below
    - 52: [![JXOS5sp.md.png](https://iili.io/JXOS5sp.md.png)](https://freeimage.host/i/JXOS5sp)
        - Binary search starts in middle and searches the half with the target, so effectively cuts the data in half each time. Thus, the maximum number of elements examined is the number of times 128 can be divided by 2. 128/2/2/2/2/2/2/2 = 7, so closest is 8.
- Questions I got wrong
    - 14: [![JXOSIea.md.png](https://iili.io/JXOSIea.md.png)](https://freeimage.host/i/JXOSIea)
        - Procedure meant to return true if numberList is increasing and false if not, so the procedure should return true IF (numberList[count] > numberList[count - 1]). Currently, the procedure repeats the check if the list is decreasing and returns true if so, and in the end returns false if the list is increasing. This is the opposite of what should be returning, so swapping the two RETURN fixes the program.
        - B is wrong because the procedure is meant to return true only if the entire list is increasing, and changing the < into >= would make every subsequent larger value return true which is not the intention. 
    - 43: [![JXOSAzv.md.png](https://iili.io/JXOSAzv.md.png)](https://freeimage.host/i/JXOSAzv)
        - Keylogging is tracking/recording keystroke entryies made on a computer, so track whatever a user types basically. Installing a program to record what a user inputs, by typing on their computer, would thus be keylogging.
    - 44: [![JXOSz5g.md.png](https://iili.io/JXOSz5g.md.png)](https://freeimage.host/i/JXOSz5g)
        - Overflow errors result in a number not being able to be represented properly (typically shows a massive negative number which is the maximum number that can be represented). Rounding errors would result in mathematically imprecise values, not overflow errors.
    - 47: [![JXOSRXR.md.png](https://iili.io/JXOSRXR.md.png)](https://freeimage.host/i/JXOSRXR)
        - Program meant to return true if have rating above 4 and below $30 (either lo and med) --> so avgRating >= 4.0 AND ((prcRange="lo") OR (prcRange="med"))
    - 57: [![JXOSYqN.md.png](https://iili.io/JXOSYqN.md.png)](https://freeimage.host/i/JXOSYqN)
        - The two PROCESSORS run in parallel (longest one determines overall time), but WITHIN the processor the procedures run right after each other (time is additive). Thus, to minimize the time, the overall processors should have the longest one be the shortest, but the time is the two time of the processes added together. As a result, the best combination is P and Q (30s + 10s = 40s) on one and R and S (20s + 15s = 35s) on the other so the overall time is 40s. 

> Hacks
- See MCQ 2020 Frequently Missed Questions