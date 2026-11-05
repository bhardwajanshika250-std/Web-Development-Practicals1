# Lab 4: Divs, Attributes and a Small Fix

## 1. Practical Aim
To group parts of a page with div elements, add a data attribute, and fix the errors in a broken HTML page.

## 2. Theoretical Background
- **Div Element (`<div>`):** A generic block-level container used to group sections of a webpage together for layout structuring.
- **Classes (`class=""`):** Used to apply styling or group multiple elements under a specific identifier.
- **Data Attributes (`data-*`):** Custom HTML attributes that allow developers to store extra proprietary information directly on elements without affecting page rendering.
- **HTML Syntax Integrity:** Ensuring all opening tags like `<h1>` and `<p>` are properly closed with `</h1>` and `</p>` to prevent broken page parsing.

## 3. Pre-requisites & Tools Used
- Visual Studio Code (Code Editor)
- Modern Web Browser (Google Chrome / Edge)
- Windows OS File Directory System

## 4. Step-by-Step Procedure
1. Created `layout.html` containing three `<div>` blocks structured with classes: `header`, `main`, and `footer`.
2. Created `attributes.html` featuring a `<div>` with `id="profile"` containing a paragraph with a custom `data-topic="hobbies"` attribute.
3. Identified unclosed `<h1>` and `<p>` tags in the provided template, corrected the syntax errors, and saved it as `attendance-fixed.html`.
4. Captured and verified browser output screenshots for all three tasks and saved them into the `lab-4/images/` directory.

## 5. Command Log / Source Code

### Task 1: `layout.html`
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page Layout</title>
</head>
<body>
    <div class="header">
        <h1>Header Section</h1>
    </div>

    <div class="main">
        <p>Main content area goes here.</p>
    </div>

    <div class="footer">
        <p>Footer Section - All Rights Reserved</p>
    </div>
</body>
</html>
6. Screenshots & Output Evidence
Task 1 Output: ![Task 1 Layout](images/task1.png)

Task 2 Output: ![Task 2 Attributes](images/task2.png)

Task 3 Output: ![Task 3 Attendance Fixed](images/task3.png)

7. Key Learning Outcomes
Understood how to divide webpage layouts cleanly using block-level <div> elements.

Learned the implementation and utility of custom data-* attributes for metadata storage.

Enhanced debugging skills by locating and resolving unclosed HTML tags.

8. Common Errors & Troubleshooting
Unclosed Tag Errors: Forgetting to close tags (like <p>Asha: 92%</p>) leads to cascading formatting distortion. Fixed by properly closing every tag.

Visual Visibility of Data Attributes: Custom data attributes like data-topic="hobbies" do not display visible text on the rendered webpage by default; their presence can be verified via Browser Developer Tools (Inspect Element).

9. Viva / Interview Questions
Q: What is the primary purpose of the <div> tag in HTML?

A: It is a generic container used to group block-level elements together to apply layout structure or styling.

Q: How do data-* attributes behave in browsers?

A: They are hidden from standard user view on the rendered page, but can be easily accessed and manipulated using JavaScript or CSS.

10. Submission Checklist
[x] Task 1 (layout.html) code & screenshot

[x] Task 2 (attributes.html) code & screenshot

[x] Task 3 (attendance-fixed.html) code & screenshot

[x] Complete README documentation


---









