---
layout: post
title: Authorization Failed Page
hide: true
description: Authorization failed page for JWT authentication
permalink: /authorizationfail
---

<body class="authorizationfailed">
    <!-- Failure Screen -->
    <h1 class="bigtitle">Error 403: Authorization failed!</h1>
    <!-- Prompt to go back to login page -->
    <h2 class="smalltitle">Please click the button below to go back to the login page:</h2>
    <button class="buttons" onclick="backtologin()">Back to Login</button>
    <script>
        function backtologin() {
            window.location.href = "{{site.baseurl}}/loginpage"
        }
    </script>
</body>