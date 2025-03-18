### Basics of HTML, CSS, and JS : Profile Page

**Objective:** Introduce students to basic HTML, CSS, and JavaScript concepts and help them apply their knowledge by building a simple project by the end of the lesson.

---

#### **1. Introduction**

- **What is HTML?**

  - Stands for HyperText Markup Language.
  - Defines the structure of a webpage using elements enclosed in tags (e.g., `<h1>content</h1>`, `<p>paragraph</p>`).
  - Example: Think of HTML as the "skeleton" of a website.

- **What is CSS?**

  - Stands for Cascading Style Sheets.
  - Adds style to the webpage, such as colors, layouts, and fonts.
  - Example: Think of CSS as the "skin and clothes" that make the skeleton visually appealing.

- **What is JavaScript?**

  - A programming language that makes the webpage interactive.
  - Example: JavaScript is the "brain" that allows the webpage to respond to user actions (e.g., clicking a button).

- **What Will We Build Today?**
  - Students will create a simple **Personal Profile Page** featuring their name, a short bio, and a button that shows a greeting message when clicked.

---

#### **2. HTML Basics**

- **What is HTML and How It Works?**

  - HTML uses tags to define the structure and content of a webpage.
  - Tags usually come in pairs, like `<p>` (opening tag) and `</p>` (closing tag).

- **Structure of an HTML Document:**

  - `<!DOCTYPE html>`: Declares the document type as HTML5.
  - `<html>`: The root element that wraps all the content on the page.
  - `<head>`: Contains metadata about the document, such as the title.
  - `<body>`: Contains the visible content of the webpage.

- **Common HTML Tags:**

  - **Headings (`<h1>` to `<h6>`)**: Define headings, with `<h1>` being the largest and `<h6>` the smallest.
    - Example: `<h1>Hello, World!</h1>`
  - **Paragraphs (`<p>`)**: Add text content.
    - Example: `<p>This is a paragraph.</p>`
  - **Lists (`<ul>` for unordered, `<ol>` for ordered)**: Create bullet points or numbered lists.
    - Example:
      ```html
      <ul>
        <li>Item 1</li>
        <li>Item 2</li>
      </ul>
      ```
  - **Images (`<img>`)**: Embed images using the `src` attribute.
    - Example: `<img src="profile.jpg" alt="Profile Picture">`
  - **Links (`<a>`)**: Create hyperlinks using the `href` attribute.
    - Example: `<a href="https://example.com">Visit Example</a>`
  - **Buttons (`<button>`)**: Add clickable buttons.
    - Example: `<button>Click Me</button>`

- **Hands-On Activity:**
  - Students create a simple HTML file:
    ```html
    <!DOCTYPE html>
    <html>
      <head>
        <title>My Profile</title>
      </head>
      <body>
        <h1>Welcome to My Profile</h1>
        <p>Hello! My name is [Your Name].</p>
        <button>Click Me</button>
      </body>
    </html>
    ```

---

#### **3. CSS Basics**

- **What is CSS and Its Purpose?**

  - CSS stands for Cascading Style Sheets and is used to style the visual elements of a webpage.
  - It can be written in three ways:
    1. Inline CSS (inside an HTML tag): `<p style="color: red;">Hello!</p>`.
    2. Internal CSS (within a `<style>` block inside `<head>`).
    3. External CSS (in a separate file linked with `<link>`).

- **How to Link a CSS File:**

  - Use the `<link>` tag in the `<head>` section:
    ```html
    <link rel="stylesheet" href="styles.css" />
    ```

- **CSS Basics:**

  - **Selectors:** Define which elements to style.
    - Element selectors: `p {}`
    - Class selectors: `.class-name {}`
    - ID selectors: `#id-name {}`
  - **Common Properties:**
    - **Color:** `color`, `background-color`
    - **Fonts:** `font-family`, `font-size`
    - **Spacing:** `margin`, `padding`
    - **Borders:** `border`, `border-radius`

- **Hands-On Activity:**
  - Add styling to the profile:
    ```css
    body {
      font-family: Arial, sans-serif;
      background-color: #f0f0f0;
      color: #333;
      text-align: center;
      padding: 20px;
    }
    button {
      padding: 10px 20px;
      background-color: #007bff;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    button:hover {
      background-color: #0056b3;
    }
    ```

---

#### **4. JavaScript Basics**

- **What is JavaScript?**

  - JavaScript is a programming language that makes webpages dynamic and interactive.
  - It runs in the browser and can manipulate HTML and CSS.

- **How to Add JavaScript to an HTML File:**

  - Use the `<script>` tag at the bottom of the `<body>` section:
    ```html
    <script src="script.js"></script>
    ```

- **JavaScript Basics:**

  - **Variables:** Store data.
    - Example: `let message = "Hello!";`
  - **Functions:** Perform actions.
    - Example: `function greet() { alert("Hello!"); }`
  - **Event Listeners:** React to user actions.
    - Example: `button.addEventListener("click", greet);`
  - **Accessing HTML Elements:**
    - Example: `document.querySelector("button")` selects a button element.

- **Hands-On Activity:**
  - Add interactivity to the button:
    ```javascript
    document.querySelector("button").addEventListener("click", function () {
      alert("Hello! Welcome to my profile!");
    });
    ```

---

#### **5. Build a Mini-Project**

- **Project Goal:** Create a simple **Personal Profile Page**.
- **Features:**

  - Name, short bio, and favorite image using HTML.
  - Styling to make it visually appealing with CSS.
  - A button that displays a custom greeting message using JavaScript.

- **Example Structure:**

  ```html
  <!DOCTYPE html>
  <html>
    <head>
      <title>My Profile</title>
      <link rel="stylesheet" href="styles.css" />
    </head>
    <body>
      <h1>Hi, I'm [Your Name]!</h1>
      <p>I love learning web development.</p>
      <img src="profile.jpg" alt="My Picture" width="150" />
      <button>Say Hello</button>

      <script src="script.js"></script>
    </body>
  </html>
  ```

---

#### **6. Review and Q&A**

- Recap what they learned:
  - **HTML:** Defines the structure.
  - **CSS:** Adds style and design.
  - **JavaScript:** Adds interactivity.
- Answer questions and troubleshoot issues.

---

### **Homework Assignment**

**Task:** Build a simple **"About My Favorite Hobby" webpage** on your own.

- **Requirements:**
  - Use **HTML** to create:
    - A title for the page.
    - A paragraph explaining your hobby.
    - An image representing your hobby.
    - A button labeled "Learn More".
  - Use **CSS** to style the page:
    - Add a background color, padding, and font styling.
    - Style the button with a hover effect.
  - Use **JavaScript** to add interactivity:
    - When the button is clicked, display a message (e.g., "I hope you enjoyed learning about my hobby!").

Encourage students to share their projects or upload them to a GitHub repository.

## variable and file naming convention

if you choose one. stick to that one in current project

snake_case -> best_variable
used alot in python

camelCase -> bestVariable
use a lot in javascript

PascalCase -> BestVariable
used when naming classes in python or javascript or any other language

SCREAMING_CASE -> BEST_VARIABLE
used when naming a constant variable tha will not change througout your program
SERVER_URL = "http://api.something.com";
LANGUAGE = ["en", "ko", "es"];

extras
starting variable with underscore usualy means throw away variable taht wil be used only once
const randomUsers = []
const \_randomUsers = [...randomUsers];

later in typescript interface will always start with I
IRandomUser {
}

type varible is always done pascal cased
