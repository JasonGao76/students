---
toc: true
comments: false
layout: post
title: Login Page
description: Frontend login page for JWT authentication
type: tangibles
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
    <input type="text" name="uid" id="uid" required><br>
    <label for="inputpassword" class="inputpassword">Enter your password here: </label><br>
    <input type="password" name="password" id="password" required><br>
    <button onclick="login()">Submit</button>
    <script type="module">
        import { uri, options } from '{{site.baseurl}}/assets/js/api/config.js';
        // placeholder
        function login() {
            var username = document.getElementById('uid').value;
            var password = document.getElementById('password').value;
            var url = uri + '/api/users/authenticate'
            var requestbody = {
                uid: username,
                password: password,
            };
            //e
            var authOptions = {
                ...options,
                method: 'POST',
                cache: 'no-cache',
                body: JSON.stringify(requestbody)
            }
            //e
            fetch(url, authOptions)
            .then(response => {
                if (!response.ok) {
                    const errorMsg = 'Login error: ' + response.status;
                    console.log(errorMsg);
                    return;
                }
                window.location.href = "{{site.baseurl}}/data/database";
            })
            .catch(err => {
                console.error(err);
            });
        };
        //e
        window.login = login;
    </script>
</body>