---
layout: post
title: Character Creation Page
hide: true
description: Character creation page for JWT authentication
permalink: /charactercreation
---

<body class="charactercreation">
    <!-- Failure Screen -->
    <h1 class="bigtitle">Create Your Character</h1>
    <h2 class="middletitle">Make your character here!</h2>
    <!-- Section 1: Name and class drop down selection -->
    <h2 class="smalltitle">Name:</h2>
    <input type="text" name="name" id="name" required><br>
    <h2 class="smalltitle">Class:</h2><br>
    <select id="class" name="class">
        <option value="knight">Knight</option>
        <option value="mage">Mage</option>
        <option value="rogue">Rogue</option>
        <option value="grandwizard">Grand Wizard</option>
    </select>
    <!-- Submit button -->
    <br>
    <button class="buttons" onclick="window.location.href='{{site.baseurl}}/charactercreation'">Submit</button>
    <script>
    </script>
</body>