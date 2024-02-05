---
layout: post
title: Signup Page
hide: true
description: Sign up page for JWT authentication
permalink: /signup
---

<body class="signup">
    <!-- Signup Screen -->
    <h1 class="bigtitle">Signup Here!</h1>
    <!-- Prompt information for signup -->
    <h2 class="mediumtitle">Please enter information for the user you would like to create!</h2>
    <label for="inputnane" class="smalltitle">Name:</label><br>
    <input type="text" name="name" id="name" required><br>
    <label for="inputusername" class="smalltitle">Uid:</label><br>
    <input type="text" name="uid" id="uid" required><br>
    <label for="inputpassword" class="smalltitle">Password:</label><br>
    <input type="password" name="password" id="password" required><br>
    <label for="inputdob" class="smalltitle">Date of Birth ("yyyy-mm-dd" format all in numbers):</label><br>
    <input type="text" name="dob" id="dob" required><br>
    <label for="inputmonth" class="smalltitle">Birth month:</label><br>
    <input type="text" name="month" id="month" required><br>
    <!-- Submit Button -->
    <button class="buttons" onclick="signup()">Submit</button>  
    <!-- Button to go back to login page -->
    <h2 class="mediumtitle">Or, go back to login here</h2>
    <button class="buttons" onclick="window.location.href='{{site.baseurl}}/signup'">Back to Login</button>
    <script type="module">
        import { uri, options } from '{{site.baseurl}}/assets/js/api/config.js';
        function signup() {
            // Set endpoint
            const url = uri + '/api/users/';
            // Create body for request
            const body = {
            name: document.getElementById("name").value,
            uid: document.getElementById("uid").value,
            password: document.getElementById("password").value,
            dob: document.getElementById("dob").value,
            month: document.getElementById("month").value
            };
            // Create options for authorization
            const authOptions = {
            ...options,
            method: 'POST',
            cache: 'no-cache',
            body: JSON.stringify(body)
            };
            // Fetch request
            fetch(url, authOptions)
            .then(response => {
                if (!response.ok) {
                    const errorMsg = 'Signup error: ' + response.status;
                    console.log(errorMsg);
                    return;
                }
                window.location.href = "{{site.baseurl}}/data/database";
            })
            .catch(err => {
                console.error(err);
            });
        };
        window.signup = signup;
    </script>
</body>