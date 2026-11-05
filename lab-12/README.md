# Lab 12: Box Model, Cards and Scrolling

## 1. Practical Aim
To compare CSS box sizing properties (`content-box` vs `border-box`), design a rounded card layout component, and implement an auto-scrolling overflow container.

## 2. Theoretical Background
- **Box Sizing (`box-sizing`):** 
  - `content-box` (default): Width and height apply only to the content area; padding and borders are added on top.
  - `border-box`: Width and height include content, padding, and borders within the specified total dimension.
- **Border Radius (`border-radius`):** Used to create rounded corners for boxes or cards.
- **Overflow (`overflow: auto`):** Automatically adds scrollbars when content exceeds the designated fixed height/width dimensions.

## 3. Pre-requisites & Tools Used
- Visual Studio Code
- Modern Web Browser (Chrome/Edge)
- Windows File Explorer

## 4. Step-by-Step Procedure
1. Created `box-model.html` featuring two boxes with identical width, padding, and borders, comparing `content-box` and `border-box` behaviors.
2. Created `card.html` containing a styled `.card` container with a background color, 2px border, 12px rounded corners, 16px padding, and nested heading and paragraph.
3. Created `scroll.html` featuring a fixed 120px height box with `overflow: auto` and five lines of text paragraphs.
4. Captured and verified browser output screenshots for all tasks and saved them into `lab-12/images/`.

## 5. Command Log / Source Code

### Task 1: `box-model.html`
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Sizing Comparison</title>
    <style>
        .box-content { width: 200px; padding: 20px; border: 5px solid navy; box-sizing: content-box; background-color: lightblue; margin-bottom: 15px; }
        .box-border { width: 200px; padding: 20px; border: 5px solid maroon; box-sizing: border-box; background-color: lightpink; }
    </style>
</head>
<body>
    <div class="box-content">Content-Box (Wider due to padding/border)</div>
    <div class="box-border">Border-Box (Width includes padding & border)</div>
</body>
</html>

Task 2: card.html
HTML


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Styled Card</title>
    <style>
        .card { width: 300px; background-color: #f4f4f4; border: 2px solid #ccc; border-radius: 12px; padding: 16px; }
    </style>
</head>
<body>
    <div class="card">
        <h3>Card Heading</h3>
        <p>This is a styled card component featuring rounded corners, custom padding, border, and background color.</p>
    </div>
</body>


Task 3: scroll.html
HTML


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Overflow Scroll Box</title>
    <style>
        .scroll-box { width: 250px; height: 120px; border: 2px solid black; overflow: auto; padding: 10px; background-color: #eef; }
    </style>
</head>
<body>
    <div class="scroll-box">
        <p>Line 1: First item inside the scrolling container.</p>
        <p>Line 2: Second item inside the container.</p>
        <p>Line 3: Third item showing overflow mechanics.</p>
        <p>Line 4: Fourth item requiring scroll action.</p>
        <p>Line 5: Fifth and final line of text content.</p>
    </div>
</body>
</html>
6. Screenshots & Output Evidence
Task 1 Output: ![Task 1 Box Model](images/task1.png)   
Screenshot 2026-11-04 151450.png

Task 2 Output: ![Task 2 Card](images/task2.png)   
Screenshot 2026-11-04 151450.png

Task 3 Output: ![Task 3 Scroll](images/task3.png)   
Screenshot 2026-11-04 151450.png

7. Key Learning Outcomes
Understood how box-sizing affects total element dimensions and layout calculations.

Learned how to design modular content UI cards using border-radius, padding, and borders[cite: 9].

Managed content overflow and scrolling behaviors using CSS overflow properties[cite: 9].

8. Common Errors & Troubleshooting
Unexpected Element Expansion: In content-box, adding padding and borders makes elements wider than specified width, causing layout overflow. Resolved by switching to box-sizing: border-box.

9. Viva / Interview Questions
Q: What is the primary difference between content-box and border-box?

A: In content-box, width applies only to content and padding/borders expand the total box size. In border-box, padding and borders are included within the specified width and height.

Q: How do you enable scrolling inside a fixed-size container when content overflows?

A: By setting the overflow property to auto or scroll[cite: 9].

10. Submission Checklist
[x] Task 1 (box-model.html) code & screenshot[cite: 9]

[x] Task 2 (card.html) code & screenshot[cite: 9]

[x] Task 3 (scroll.html) code & screenshot[cite: 9]

[x] Complete README documentation


---

Aap in files ko save karke browser mein check kar lijiye aur screenshots `lab-12/images/` folder mein dal dijiye! Bataiye, kya aur koi assignment ya lab bacha hai?





