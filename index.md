Assignment Number- 1.2  
Subject: Web Development  

## 1. Aim

To set up a web development environment on a computer, install the required tools, create a basic webpage, and run it in a web browser using Live Server.

## 2. Software and Tools Required

1. Visual Studio Code (VS Code)
2. Node.js LTS
3. Live Server extension for VS Code
4. Prettier - Code formatter extension for VS Code
5. A modern web browser (such as Chrome, Edge, or Firefox)

## 3. Procedure

### Step 1: Install Visual Studio Code

1. Visit the official website: https://code.visualstudio.com/Download
2. Download the installer for your operating system.
3. Run the installer and complete the installation.
4. Open Visual Studio Code.

### Step 2: Install Node.js LTS

1. Visit the official website: https://nodejs.org/en/download
2. Download the **LTS (Long-Term Support)** version for your operating system.
3. Run the installer and follow the setup instructions.
4. Keep the default options unless your instructor or administrator specifies otherwise.
5. After installation, open a new terminal.

### Step 3: Install VS Code Extensions

1. Open VS Code.
2. Open the Extensions panel using `Ctrl + Shift + X`.
3. Search for **Live Server** and install it (Ritwick Dey).
4. Search for **Prettier - Code formatter** and install it.
5. Confirm that both extensions are installed.

### Step 4: Create the Project Folder

Create a folder named:

`web-development-practice`

Inside this folder, create the following three files:

```text
web-development-practice/ index.html ,style.css, script.js

### Step 5: Write the HTML Code

Save the following code in `index.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Webpage</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <main class="container">
        <h1>Welcome to My First Webpage!</h1>
        <p class="student-name">Student Name: Vivek</p>
        <p class="assignment">
            This webpage was created for Assignment 1.2:
            Development Environment Setup.
        </p>
        <button id="helloButton" type="button">Click Me</button>
        <p id="message" aria-live="polite"></p>
    </main>
    <script src="script.js"></script>
</body>
</html>
```

### Step 6: Write the CSS Code

Save the following code in `style.css`:

```css
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    min-height: 100vh;
    display: grid;
    place-items: center;
    padding: 24px;
    font-family: Arial, sans-serif;
    background: #eef2ff;
    color: #1f2937;
}

.container {
    width: min(100%, 680px);
    padding: 40px 28px;
    text-align: center;
    background: #ffffff;
    border-radius: 16px;
    box-shadow: 0 12px 30px rgba(31, 41, 55, 0.12);
}

h1 {
    margin-top: 0;
    color: #1d4ed8;
}

.student-name {
    font-weight: bold;
}

.assignment {
    line-height: 1.6;
}

button {
    padding: 12px 22px;
    border: none;
    border-radius: 8px;
    background: #1d4ed8;
    color: #ffffff;
    font-size: 16px;
    cursor: pointer;
}

button:hover {
    background: #1e40af;
}

#message {
    min-height: 24px;
    margin-bottom: 0;
    color: #166534;
    font-weight: bold;
}
```

### Step 7: Write the JavaScript Code

Save the following code in `script.js`:

```javascript
const helloButton = document.getElementById("helloButton");
const message = document.getElementById("message");

helloButton.addEventListener("click", () => {
    message.textContent = "Great! HTML, CSS, and JavaScript are working.";
});
```

### Step 8: Verify Node.js and npm

In VS Code, select **Terminal → New Terminal** and run these commands separately:

```bash
node -v
npm -v
```

Both commands should print version numbers. The exact versions depend on the version installed on the computer. If the commands are not recognized, restart the terminal or VS Code and try again.

### Step 9: Run the Webpage Using Live Server

1. Open `index.html` in VS Code.
2. Right-click inside the editor.
3. Select **Open with Live Server**.
4. The webpage should open in the default browser.
5. Click the **Click Me** button and confirm that a message appears.
6. If Live Server does not appear, confirm that its extension is installed and reload VS Code.

## 4. Expected Output

The browser should display a centered webpage containing:

- The heading “Welcome to My First Webpage!”
- The student name
- The assignment description
- A “Click Me” button
- A message after the button is clicked

## 5. Screenshot Evidence

**Attach your own screenshots in this section before submitting.**

1. **Screenshot 1 — VS Code:** Show the `web-development-practice` folder, the three project files, and the installed Live Server and Prettier extensions.
2. **Screenshot 2 — Node.js and npm:** Show the terminal with the results of `node -v` and `npm -v`.
3. **Screenshot 3 — Browser output:** Show the webpage running through Live Server. If possible, click the button so the JavaScript message is visible.

> Important: These screenshots must be captured from your own computer after you complete the steps. Do not submit empty placeholders as proof of installation.

## 6. Result

The web development project was created with `index.html`, `style.css`, and `script.js`. Node.js and npm were checked using terminal commands, and the webpage was run in a browser using Live Server.

## 7. Conclusion

This assignment provides practical experience in preparing a basic web development environment. It introduces Visual Studio Code, Node.js, npm, Live Server, and Prettier, and demonstrates how HTML, CSS, and JavaScript work together to create an interactive webpage.
