# Lab 8: Sign-Up Forms and Choices

## 1. Practical Aim
To build labelled HTML forms incorporating text, email, password fields, radio buttons, dropdown select menus, placeholders, and validation attributes.

## 2. Theoretical Background
- **Form Element (`<form>`):** Container for grouping interactive input controls. Attributes include `action` and `method`.
- **Label Element (`<label>`):** Provides a caption for a form control, linked via the `for` attribute matching the input's `id`.
- **Input Types (`type="text"`, `type="email"`, `type="password"`, `type="radio"`):** Define the behavioral and formatting nature of input fields.
- **Select Dropdown (`<select>` & `<option>`):** Creates a collapsible menu of selectable options.
- **Validation & Placeholders (`required`, `placeholder`):** Enforces field completion before form submission and displays hint text inside empty inputs.

## 3. Pre-requisites & Tools Used
- Visual Studio Code
- Modern Web Browser (Chrome/Edge)
- Windows File Explorer

## 4. Step-by-Step Procedure
1. Created `signup.html` containing a form with `method="post"` and `action="thanks.html"`, featuring labelled fields for full name, email, and password.
2. Created `choices.html` featuring radio buttons for gender selection (Female/Male) and a dropdown selection list for courses (BCA and B.Tech).
3. Created `signup-required.html` containing mandatory input fields configured with `required` and `placeholder` attributes along with a submit button.
4. Captured and verified browser output screenshots for all tasks and saved them into `lab-8/images/`.

## 5. Command Log / Source Code

### Task 1: `signup.html`
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sign Up Form</title>
</head>
<body>
    <h1>Sign Up</h1>
    <form action="thanks.html" method="post">
        <div>
            <label for="fullname">Full Name:</label><br>
            <input type="text" id="fullname" name="fullname">
        </div>
        <br>
        <div>
            <label for="email">Email:</label><br>
            <input type="email" id="email" name="email">
        </div>
        <br>
        <div>
            <label for="password">Password:</label><br>
            <input type="password" id="password" name="password">
        </div>
        <br>
        <div>
            <button type="submit">Submit</button>
        </div>
    </form>
</body>
</html>

Task 2: choices.html
HTML


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Choices Form</title>
</head>
<body>
    <h1>User Choices</h1>
    <form>
        <fieldset>
            <legend>Gender</legend>
            <input type="radio" id="female" name="gender" value="Female">
            <label for="female">Female</label><br>
            <input type="radio" id="male" name="gender" value="Male">
            <label for="male">Male</label>
        </fieldset>
        <br>
        <div>
            <label for="course">Select Course:</label><br>
            <select id="course" name="course">
                <option value="bca">BCA</option>
                <option value="btech">B.Tech</option>
            </select>
        </div>
    </form>
</body>
</html>
Task 3: signup-required.html
HTML


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Required Sign Up</title>
</head>
<body>
    <h1>Required Sign Up</h1>
    <form>
        <div>
            <label for="req-name">Full Name:</label><br>
            <input type="text" id="req-name" name="req-name" placeholder="Enter your full name" required>
        </div>
        <br>
        <div>
            <label for="req-email">Email:</label><br>
            <input type="email" id="req-email" name="req-email" placeholder="Enter your email" required>
        </div>
        <br>
        <div>
            <button type="submit">Submit</button>
        </div>
    </form>
</body>
</html>
6. Screenshots & Output Evidence
Task 1 Output: ![Task 1 Sign Up](images/task1.png)   
Screenshot 2026-11-04 145114.png

Task 2 Output: ![Task 2 Choices](images/task2.png)   
Screenshot 2026-11-04 145114.png

Task 3 Output: ![Task 3 Required Sign Up](images/task3.png)[cite: 7]

7. Key Learning Outcomes
Learned how to construct structured form inputs with explicit label bindings.

Understood how radio buttons group mutually exclusive choices and how dropdowns function via <select> and <option>.

Explored native browser validation using the required attribute.

8. Common Errors & Troubleshooting
Unlinked Labels: Clicking the label text did not focus the input field. Fixed by ensuring the <label for="..."> matches the corresponding <input id="...">.

9. Viva / Interview Questions
Q: What is the purpose of the required attribute in form inputs?

A: It forces the user to fill out the input field before the form can be submitted, triggering a browser validation message if left empty[cite: 7].

Q: How do you ensure only one radio button can be selected in a group?

A: By giving all radio buttons in that group the exact same name attribute value.

10. Submission Checklist
[x] Task 1 (signup.html) code & screenshot[cite: 7]

[x] Task 2 (choices.html) code & screenshot[cite: 7]

x] Task 3 (signup-required.html) code & screenshot[cite: 7]

[x] Complete README documentation

