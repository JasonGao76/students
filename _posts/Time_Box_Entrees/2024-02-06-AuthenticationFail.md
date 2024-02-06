---
layout: post
title: Authentication Failed Page
hide: true
description: Authentication failed page for JWT authentication
permalink: /authenticationfail
---

<body class="authenticationfailed">
    <!-- Failure Screen -->
    <h1 class="bigtitle">Authentication failed!</h1>
    <h2 class="mediumtitle">Incorrect username or password!</h2>
    <!-- Prompt to go back to login page -->
    <h2 class="smalltitle">Please click the button below to go back to the login page:</h2>
    <button class="buttons" onclick="backtologin()">Back to Login</button>
    <script>
        function backtologin() {
            window.location.href = "{{site.baseurl}}/loginpage"
        }
    </script>
</body>