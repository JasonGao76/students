---
toc: true
comments: false
layout: post
title: 2020 Practice Exam 1 Blog Post
description: Blog post for assigned Collegeboard test 2020 Practice Exam 1 MCQ with notes, time taken, and corrections
type: tangibles
courses: { compsci: {week: 17} }
---

## 2020 Practice Exam 1 MCQ Notes
> Questions Googled and Notes on what Researched
- Question 4
    - Overflow error is when program gets a number, value, or variable that it can't handle
- Question 9
    - Only one to do with security is public-key, Creative Commons license allows use of some material if creator attributed, high-bandwidth has to do with speed, and redundant routing just makes sure it gets there but doesn't provide security
- Questions 11-12
    - About binary and RGB colors, IT GOES FROM HIGHEST TO LOWEST POWER OF 2
- Question 17
    - Bits can represent all 3 (integer (binary), alphanumeric character (ASCII, Unicode, other character encoding schemes), and machine language instruction (uses binary code))
- Question 35
    - Generalization of procedure is like procedural abstraction where you organize/encapsulate procedures/algorithms with names and variables or parameters
- Question 40
    - Certificate authority is a trusted entity that issues SSL certificates, verifying the authenticity of encryption keys for secure  communications
- Question 52
    - Googled to make sure answer was right, I is correct because of the conditions "REPEAT UNTIL ((hours >= 24) OR (currentPop <= 0)), II is wrong because the change in population isn't displayed per hour and isn't average change, III is wrong because it's not the total population but change in population
- Question 54
    - CollegeBoard pseudocode reference sheet link: https://apcentral.collegeboard.org/media/pdf/ap-computer-science-principles-exam-reference-sheet.pdf?course=ap-computer-science-principles. INSERT (list, i, value) shifts everything with indices greater or equal to i to the right and places value at index i. APPEND (list, value) places value at the end of list.

> General Notes
- Pseudocode uses REPEAT _ TIMES or REPEAT UNTIL _ as loop
- Logic gates: <img src="https://global.discourse-cdn.com/codecademy/original/5X/9/2/5/e/925ecf1588b896bd5e07dfd730abfb17b4c138ee.png">
- IP Addresses enable newly connected devices to the Internet to communicate on network
- Pseudocode uses CAN_MOVE for robot poblems in addition to regular movement and rotate commands
- Question 7 is interesting question with impact of flight simulations, use logic
- Pseudocode uses DISPLAY instead of print
- Question 14 is an interesting algorithm with displaying individual digits of a number from right to left
- Pseudocode uses <-- instead of =
- Questions 19-21 are statistical questions of a file storage application, use logic
- Pseudocode uses RANDOM a, b to get random number from a to b (inclusive)
- Question 31 deals with copyright, use logic
- Pseudocode uses LENGTH instead of len
- Pseudocode uses PROCUDURE instead of like a function name
- Question 36 has model and updating model to reduce runtime, use logic
- Question 39 has interesting procedure with sum of first 10 numbers of an array, and line numbers
- Question 41 is interesting procedure with trimming characters
- Question 43-44 is about routing connections and redundant routing
- Question 45 is interesting procedure with coin flipping game
- Question 48 is about phishing
- Question 50 is about algorithm runtime with a large list
- Question 53 is about crowdsourcing in a pet finding application
- Pseudocode uses MOD instead of %
- Question 55 has very interesting use of people instead of computers to run a program to calculate average height
- TCP and IP standardizes how data is exchanged over the internet (remember TCP has its handshake)
- Question 59 is about open source software, use logic since both open source software and commercial software provides free/low cost support
- Question 60 has very interesting program about finding number of unique numbers in two lists, took a while to think through it and write out some examples and test them all
- Question 64 is interesting algorithm to do multiplication by repeated addition and input results in unintended output
- Question 66 is fun algorithm to find the number of perfect numbers between two numbers and have to fix the code
- Question 64-67 are all fixing code or finding the inputs that the code doesn't return proper output
- **TOTAL TIME**: 2 hours, 19 minutes, and 7 seconds (sometimes clicked off a little bit for around 10 minutes total), so roughly 2 hours spent totally

> Corrections
- Question 26 Metadata for an image
    - <img src="https://i.postimg.cc/ZK6J0jTh/Q26.jpg">
    - Actual answer and explanation: D, A duplicate copy of the data. Metadata can be considered as the additional information for the data, making finding and working with it a lot easier. Usually it has information like the author, date created and modified, size, copyright, etc. It likely won't have another copy of the data because it would be just the actual data then and would make the file sizes way too large to be practical.
- Question 50 Reasonable time algorithms
    - <img src="https://i.postimg.cc/nhZpm7z9/Q50.jpg">
    - Actual answer and explanation: D, I, II, and III. Reasonable time to run is considered anything that is not exponential to itself or the number of elements. Regular powers (to a reasonable degree) of the number of elements, constant times number of elements, other numerical operations with number of elements, and reasonably small numbers are all considered "reasonable", only something like n^n would be considered unreasonable since it's exponential to the number of elements.
- Question 51 Creative Commons
    - <img src="https://i.postimg.cc/nhkZGzjR/Q51.jpg">
    - Actual answer and explanation: A, Creative Commons gives creators of digital content the ability to indicate how their works can be legally used and distributed, enabling broad access to digital information. Creative Commons licenses only apply to works that were published with the license, so previously copyrighted work are not eligible to be legally used and distributed under Creative Commons (I think I didn't see the "previously copyrighted work" part). Creative Commons does allow owners to explain what ways their work can and can not be used or distribtued.
- Question 60 Number of elements in one list but not both
    - <img src="https://i.postimg.cc/pdLvGHK2/Q60.jpg">
    - Actual answer and explanation: D, see above image for code. The best way to do this question is to test all the code. Assume list1 = [10, 10, 20, 30, 40, 50, 60] and list2 = [20, 20, 40, 60, 80], the output should be 3.
        - Option A: bothList = [10, 10, 20, 20, 20, 30, 40, 40, 50, 60, 60, 80], uniqueList as [10, 20, 30, 40, 50, 60, 80], so count = 12 - 7 = 5, not right
        - Option B: newList1 = [10, 20, 30, 40, 50, 60], newList2 = [20, 40, 60, 80], bothList = [10, 20, 20, 30, 40, 40, 50, 60, 60, 80], so count = 7 + 5 - 10 = 2, not right
        - Option C: newList1 = [10, 20, 30, 40, 50, 60], newList2 = [20, 40, 60, 80], bothList = [10, 20, 20, 30, 40, 40, 50, 60, 60, 80], so count = 6 + 4 - 10 = 0, not right
        - Option D: newList1 = [10, 20, 30, 40, 50, 60], newList2 = [20, 40, 60, 80], bothList = [10, 20, 20, 30, 40, 40, 50, 60, 60, 80], uniqueList = [10, 20, 30, 40, 50, 60, 80], so count = 10 - 7 = 3, right
    - I did test this with alternate lists and B worked, so I think I might've just done the math wrong for that test.