---
layout: post
title: Update Date Page
hide: true
description: Update date page for JWT authentication
permalink: /updatedata
---

<body class="updatedata">
    <!-- Failure Screen -->
    <h1 class="bigtitle">Update Data Here!</h1>
    <!-- Prompt new updated info -->
    <label for="inputnane" class="smalltitle">New Name:</label><br>
    <input type="text" name="name" id="name" required><br>
    <label for="inputusername" class="smalltitle">Uid (uid of user you want to update data for):</label><br>
    <input type="text" name="uid" id="uid" required><br>
    <label for="inputpassword" class="smalltitle">New Password:</label><br>
    <input type="password" name="password" id="password" required><br>
    <label for="inputdob" class="smalltitle">New Date of Birth ("yyyy-mm-dd" format all in numbers):</label><br>
    <input type="text" name="dob" id="dob" required><br>
    <label for="inputmonth" class="smalltitle">New Birth month:</label><br>
    <input type="text" name="month" id="month" required><br>
    <!-- Prompt to submit -->
    <h2 class="smalltitle">Submit Updated Data Here!</h2>
    <button class="buttons" onclick="updatedata()">Submit</button>
    <script type="module">
        import { uri, options } from '{{site.baseurl}}/assets/js/api/config.js';
        function updatedata(){
        // if (document.getElementById("password").value != document.getElementById("confirmpassword").value) {
        //     alert("Error: Passwords do not match.");
        //     return;
        // }
        const url = uri + '/api/users/';
        const body = {
            uid: document.getElementById("uid").value,
            password: document.getElementById("password").value,
            name: document.getElementById("name").value,
            dob: document.getElementById("dob").value,
            month: document.getElementById("month").value
        };
        const AuthOptions = {
            mode: 'cors', // no-cors, *cors, same-origin
            credentials: 'include', // include, same-origin, omit
            headers: {
                'Content-Type': 'application/json',
            },
            method: 'PUT', // Override the method property
            cache: 'no-cache', // Set the cache property
            body: JSON.stringify(body)
            };
            // fetch the API
            fetch(url, AuthOptions)
            // response is a RESTful "promise" on any successful fetch
            .then(response => {
                // check for response errors and display
                if (response.status !== 200) {
                    window.location.href = "{{site.baseurl}}/loginpage";
                }
                // valid response will contain JSON data
                response.json().then(data => {
                    window.location.href = "{{site.baseurl}}/data/database";
                })
            })
            // catch fetch errors (ie ACCESS to server blocked)
            .catch(err => {
            console.log(err)
            });
        }
        // Attach login_user to the window object, allowing access to form action
        window.updatedata = updatedata;
    </script>
</body>