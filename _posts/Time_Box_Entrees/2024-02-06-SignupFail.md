---
layout: post
title: Signup Failed Page
hide: true
description: Signup failed page for JWT authentication
permalink: /signupfail
---

<body class="signupfailed">
    <!-- Failure Screen -->
    <h1 class="bigtitle">Signup failed!</h1>
    <!-- Prompt to go back to login page -->
    <h2 class="smalltitle">Please click the button below to go back to the signup page:</h2>
    <button class="buttons" onclick="backtosignup()">Back to Signup</button>
    <script>
        function backtosignup() {
            window.location.href = "{{site.baseurl}}/signup"
        }
    </script>
</body>