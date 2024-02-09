---
layout: post
title: Character Creation Page
hide: true
description: Character creation page for JWT authentication
permalink: /charactercreation
---
<head>
    <style>
        .candle {
            max-width: 100%;
        }
        .charactercreation {
            display: flex;
            align-items: center;
        }
        .bigtitle {
            flex: 1;
            margin-right: 20px;
        }
        .mediumtitle {
            flex: 1;
            margin-right: 20px;
        }
        .smalltitle {
            flex: 1;
            margin-right: 20px;
        }
        table {
            display: none;
        }
    </style>
</head>
<body class="charactercreation">
    <!-- Failure Screen -->
    <h1 class="bigtitle">Create Your Character</h1>
    <h2 class="middletitle">Make your character here!</h2>
    <!-- Section 1: Name and class drop down selection -->
    <h2 class="smalltitle">Name:</h2>
    <input type="text" name="name" id="name" required><br>
    <h2 class="smalltitle">Class:</h2>
    <select id="class" name="class" onchange="showinfo()"> <!-- use onchange to run fetch stuff or can combine into 1 function -->
        <option value="">Pick a class</option>
        <option value="knight">Knight</option>
        <option value="mage">Mage</option>
        <option value="rogue">Rogue</option>
        <option value="shieldbearer">Shield Bearer</option>
        <option value="grandwizard">Grand Wizard</option>
    </select>
    <!-- Display data and image -->
    <div id="classInfo">
        <div id="knight-details" class="class-details" style="display: none;">
            <p>You've selected the Knight class! Strong, loyal, and determined, this class features a balance between offense and defense.</p>
        </div>
        <div id="mage-details" class="class-details" style="display: none;">
            <p>You've selected the Mage class! Intelligent and calm, this class features the ability to attack any space on the map at the cost of a lower health.</p>
        </div>
        <div id="rogue-details" class="class-details" style="display: none;">
            <p>You've selected the Rogue class! Cunning and quick, this class features the ability to move multiple spaces at the cost of a lower health.</p>
        </div>
        <div id="shieldbearer-details" class="class-details" style="display: none;">
            <p>You've selected the Shield Bearer class! Sturdy and unwavering, this class features extra health.</p>
        </div>
        <div id="grandwizard-details" class="class-details" style="display: none;">
            <p>You've selected the Grand Wizard class! This class is omnipotent, essentially unable to be beaten. Use this class for testing.</p>
        </div>
        <div class="class-details">
            <table>
                <thead>
                <tr>
                    <th>Class</th>
                    <th>Health</th>
                    <th>Attack</th>
                </tr>
                </thead>
                <tbody id="result">
                <!-- Generated data goes here -->
                </tbody>
            </table>
        </div>
    </div>
    <!-- Submit button -->
    <br>
    <button class="buttons" onclick="window.location.href='{{site.baseurl}}/charactercreation'">Submit</button>
    <img class="candle" src="https://i.postimg.cc/wj2FYHpM/candle-removebg-preview.png">
    <script>
        function showinfo() {
            var selectedclass = document.getElementById("class").value;
            var infodiv = document.getElementById("classInfo");
            // Hide all info divs initially
            var allinfodivs = document.querySelectorAll(".class-details");
            allinfodivs.forEach(function(div) {
                div.style.display = "none";
            });
            // Show the selected info div
            var selectedinfodiv = document.getElementById(selectedclass + "-details");
            if (selectedinfodiv) {
                selectedinfodiv.style.display = "block";
            }
        }
        // define fetch stuff
    </script>
</body>