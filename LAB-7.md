# Browser Exploitation Practical Guide

In this practical guide, we'll explore browser exploitation techniques, including creating a simple HTML webpage, inserting malicious JavaScript, setting up Apache2, and using the BeEF (Browser Exploitation Framework) server for executing social engineering attacks.

## 1. Build a Simple HTML Webpage

Create an HTML file (e.g., `index.html`) with the following content:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Malicious Page</title>
</head>
<body>
    <h1>Welcome to our Website!</h1>
    <p>This is a normal webpage content.</p>
</body>
</html>
```
# Inserting Malicious JavaScript

Edit the HTML file to include a script with malicious intentions:

```
<!-- Add this script within the <head> or <body> section -->
<script>
    alert('Your system has been compromised!');
    // Add more malicious actions here
</scrip
```

# Setting up Apache2 Server

Ensure Apache2 is installed on your server. Place your HTML file in the Apache root directory (e.g., /var/www/html/).

Start or restart Apache2:

`sudo service apache2 start`

# BeEF (Browser Exploitation Framework) Setup

Install BeEF on your server:

`sudo apt-get install beef-xss`

Start BeEF:

`sudo beef-xss`

Access the BeEF control panel at http://localhost:3000/ui/panel.

# Executing Social Engineering Attacks

    Send the link to your HTML page to the target.
    When the target opens the page, the malicious JavaScript executes.
    Monitor the BeEF control panel for active hooked browsers.
    Perform various social engineering attacks using BeEF.

Note: Ensure all activities are performed responsibly and within legal boundaries. Unauthorized exploitation is strictly prohibited.



