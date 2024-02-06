---
toc: true
comments: false
layout: post
title: Login Page
description: Frontend login page for JWT authentication
type: tangibles
courses: { compsci: {week: 19} }
permalink: /loginpage
---

<body class="loginfrontend">
    <!-- Welcome -->
    <h1 class="bigtitle">Welcome Back!</h1>
    <!-- Prompt for login info -->
    <h2 class="mediumtitle">Please enter your information below!</h2>
    <label for="inputusername" class="smalltitle">Enter your username here:</label><br>
    <input type="text" name="uid" id="uid" required><br>
    <label for="inputpassword" class="smalltitle">Enter your password here: </label><br>
    <input type="password" name="password" id="password" required><br>
    <button class="buttons" onclick="login()">Login</button><br>
    <h2 class="mediumtitle">Or if you need to create a user, click below to go to the signup page!</h2>
    <button class="buttons" onclick="window.location.href='{{site.baseurl}}/signup'">Go to Signup</button>
    <script type="module">
        import {uri, options} from '{{site.baseurl}}/assets/js/api/config.js';
        // placeholder
        function login() {
            var username = document.getElementById('uid').value;
            var password = document.getElementById('password').value;
            var url = uri + '/api/users/authenticate'
            var requestbody = {
                uid: username,
                password: password,
            };
            //
            var authOptions = {
                ...options,
                method: 'POST',
                cache: 'no-cache',
                body: JSON.stringify(requestbody)
            }
            //
            fetch(url, authOptions)
            .then(response => {
                if (!response.ok) {
                    const errorMsg = 'Login error: ' + response.status;
                    console.log(errorMsg);
                    window.location.href = "{{site.baseurl}}/authenticationfail";
                    return;
                }
                window.location.href = "{{site.baseurl}}/data/database";
            })
            .catch(err => {
                console.error(err);
            });
        };
        window.login = login;
    </script>
</body>