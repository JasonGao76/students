---
toc: true
comments: false
layout: post
title: Login Page
description: Frontend login page for JWT authentication
type: hacks
courses: { compsci: {week: 19} }
---

<!-- <link rel="stylesheet" href="test.css">  -->

<head>
<style>
    body {
      background-color: #a080e2 /* no work :( */
    }
</style>
</head>

<body class="loginfrontend">
    <!-- Welcome -->
    <h1 class="welcome">Welcome Back!</h1>
    <!-- Prompt for info -->
    <h2 class="promptinfo">Please enter your information below!</h2>
    <label for="inputusername" class="inputusername">Enter your username here:</label><br>
    <input type="text" class="inputusernamebox"><br>
    <label for="inputpassword" class="inputpassword">Enter your password here: </label><br>
    <input type="text" class="inputpasswordbox"><br>
    <button onclick="storeusernamepassword()">Submit</button>
    <!-- <form action="/submit_form (url for where to send info to)" method="post">
        <label for="userInput">Enter something:</label>
        <input type="text" id="userInput" name="userInput">
        <button type="submit">Submit</button>
    </form> -->
    <script>
        function storeusernamepassword() {
            var username = document.getElementById('inputusername');
            var password = document.getElementById('inputpassword');
            console.log(username)
            console.log(password)
        }
    </script>
</body>