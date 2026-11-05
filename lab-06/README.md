# Lab 6: Types of HTML Lists

## 1. Practical Aim
To create a bulleted unordered list, a numbered list with a nested list, and a description list in HTML.

## 2. Theoretical Background
- **Unordered List (`<ul>`):** Used to create a bulleted list where items order does not matter. Each item is defined by `<li>`.
- **Ordered List (`<ol>`):** Used to create a numbered/sequenced list.
- **Nested Lists:** Placing an `<ul>` or `<ol>` inside an `<li>` element to create sub-lists.
- **Description List (`<dl>`):** Used to display name/value pairs or terms and definitions using `<dt>` (term) and `<dd>` (description).

## 3. Pre-requisites & Tools Used
- Visual Studio Code
- Modern Web Browser (Chrome/Edge)
- Windows File Explorer

## 4. Step-by-Step Procedure
1. Created `shopping-list.html` featuring a heading and an unordered list (`<ul>`) containing Notebook, Pen, and Bag.
2. Created `canteen-menu.html` featuring a numbered list (`<ol>`) with a nested ordered list under Sandwich containing Cheese and Vegetable.
3. Created `faq.html` containing a description list (`<dl>`) with question terms (`<dt>`) and answers (`<dd>`).
4. Captured and verified browser output screenshots for all three tasks and saved them into `lab-6/images/`.

## 5. Command Log / Source Code

### Task 1: `shopping-list.html`
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shopping List</title>
</head>
<body>
    <h1>Shopping List</h1>
    <ul>
        <li>Notebook</li>
        <li>Pen</li>
        <li>Bag</li>
    </ul>
</body>
</html>
Task 2: canteen-menu.html
HTML


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Canteen Menu</title>
</head>
<body>
    <h1>Canteen Menu</h1>
    <ol>
        <li>Beverages</li>
        <li>Sandwich
            <ol>
                <li>Cheese</li>
                <li>Vegetable</li>
            </ol>
        </li>
    </ol>
</body>
</html>
Task 3: faq.html
HTML


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FAQ</title>
</head>
<body>
    <h1>Library FAQ</h1>
    <dl>
        <dt>How many books can I borrow?</dt>
        <dd>You can borrow up to 5 books at a time.</dd>
        <dt>Is library open on Sunday?</dt>
        <dd>No, the library remains closed on Sundays.</dd>
    </dl>
</body>
</html>
6. Screenshots & Output Evidence
Task 1 Output: ![Task 1 Shopping List](images/task1.png)

Task 2 Output: ![Task 2 Canteen Menu](images/task2.png)

Task 3 Output: ![Task 3 FAQ](images/task3.png)

7. Key Learning Outcomes
Understood how to structure content using unordered, ordered, and nested lists.

Learned how to use description lists for FAQs or glossary data.

8. Common Errors & Troubleshooting
Improper Nesting: Forgetting to place the nested list inside an <li> tag can break hierarchy. Fixed by nesting properly.

9. Viva / Interview Questions
Q: What is the difference between <ul> and <ol>?

A: <ul> creates an unordered bulleted list, whereas <ol> creates a numbered/ordered sequential list.

Q: Which tags are used inside a description list (<dl>)?

A: <dt> is used for the description term (heading/question), and <dd> is used for the description data (answer/definition).

10. Submission Checklist
[x] Task 1 (shopping-list.html) code & screenshot[cite: 6]

[x] Task 2 (canteen-menu.html) code & screenshot[cite: 6]

[x] Task 3 (faq.html) code & screenshot[cite: 6]

[x] Complete README documentation






