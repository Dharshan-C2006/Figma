# Ex09 Event Registration Web Application
# Date:05-5-2025
# AIM:
To design, develop and deploy a web application for event registration.

# DESIGN STEPS:
## Step 1:
Create a new frame.

## Step 2:
Select any one preset size of your choice.

## Step 3:
Select the shapes you need.

## Step 4:
Import images as needed.

## Step 5:
Create pages based on your need and link them.

## Step 6:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# DESIGN TOOL:
Figma

# CODE:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Sports Event Registration</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: Arial, sans-serif;
      background-color: #000;
      color: white;
      text-align: center;
    }
    .screen {
      display: none;
      padding: 20px;
    }
    .active {
      display: block;
    }
    .header {
      background-color: #002244;
      padding: 10px;
      font-size: 14px;
      font-weight: bold;
    }
    .buttons {
      margin-top: 20px;
    }
    button {
      padding: 10px 20px;
      margin: 10px;
      border: none;
      color: white;
      cursor: pointer;
      font-weight: bold;
    }
    .btn-exit { background-color: red; }
    .btn-register { background-color: blue; }
    .btn-next { background-color: #00aaff; }
    .sports-list {
      text-align: left;
      padding-left: 30%;
    }
    form input {
      width: 80%;
      padding: 8px;
      margin: 10px 0;
    }
    .thankyou {
      margin-top: 50px;
      font-size: 24px;
      font-weight: bold;
    }
    .subtext {
      font-size: 12px;
      margin-top: 10px;
    }
  </style>
</head>
<body>

  <!-- Header -->
  <div class="header">
    SAVEETHA ENGINEERING COLLEGE - TNEA CODE: 1216
  </div>

  <!-- Screen 1: Landing -->
  <div class="screen active" id="screen1">
    <h2>SPORTS EVENT</h2>
    <img src="college.jpg" alt="College" style="width: 200px; height: 200px; border-radius: 50%; margin-top: 20px;" />
    <div class="buttons">
      <button class="btn-exit">EXIT</button>
      <button class="btn-register" onclick="showScreen(2)">REGISTER</button>
    </div>
  </div>

  <!-- Screen 2: Sports List -->
  <div class="screen" id="screen2">
    <h2>SPORTS EVENT</h2>
    <div class="sports-list">
      <p>› Cricket</p>
      <p>› Badminton</p>
      <p>› Volley Ball</p>
      <p>› Basket Ball</p>
      <p>› Swimming</p>
      <p>› 100 mts</p>
      <p>› 1000 mts</p>
      <p>› Foot Ball</p>
      <p>› Handball</p>
    </div>
    <div class="buttons">
      <button class="btn-next" onclick="showScreen(3)">Register For Event</button>
    </div>
  </div>

  <!-- Screen 3: Registration Form -->
  <div class="screen" id="screen3">
    <h2>REGISTER THIS FORM:</h2>
    <form onsubmit="event.preventDefault(); showScreen(4);">
      <input type="text" placeholder="Name" required><br>
      <input type="number" placeholder="Age" required><br>
      <input type="text" placeholder="Gender" required><br>
      <input type="tel" placeholder="Phone" required><br>
      <input type="text" placeholder="Sports" required><br>
      <input type="text" placeholder="Address" required><br>
      <input type="text" placeholder="Department" required><br>
      <input type="text" placeholder="Sport" required><br>
      <button type="submit" class="btn-register">Submit</button>
    </form>
  </div>

  <!-- Screen 4: Thank You -->
  <div class="screen" id="screen4">
    <div class="thankyou">THANK YOU !!!!</div>
    <div class="subtext">...VENUE WILL BE UPDATED SOON...</div>
  </div>

  <script>
    function showScreen(n) {
      document.querySelectorAll('.screen').forEach(screen => screen.classList.remove('active'));
      document.getElementById('screen' + n).classList.add('active');
    }
  </script>
</body>
</html>

```
# OUTPUT:

![alt text](<WhatsApp Image 2025-05-20 at 10.03.49_adeab69e.jpg>)
# RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
