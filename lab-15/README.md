# Lab 15: Responsive Pages with Media Queries

## 1. Practical Aim
To build responsive web designs using a mobile-first CSS layout approach, scalable images (`max-width: 100%`), media queries (`@media (min-width: 600px)`), and relative typography scaling using `rem` units.

## 2. Theoretical Background
- **Mobile-First Approach:** Writing base CSS for mobile/small viewports first, then enhancing the layout for desktop screens using `min-width` media queries.
- **Responsive Images:** Setting `max-width: 100%` and `height: auto` ensures images shrink to fit smaller screens without breaking layout boundaries or distorting aspect ratios.
- **Responsive Typography (`rem`):** Utilizing relative root-based units in combination with media queries allows smooth scale adjustments across viewport sizes.

## 3. Pre-requisites & Tools Used
- Visual Studio Code
- Modern Web Browser (Chrome/Edge)
- Windows File Explorer

## 4. Step-by-Step Procedure
1. Created `mobile-first.html` configured with `<meta name="viewport">`, styling card containers to stack vertically on mobile and display side-by-side at 600px+ breakpoints.
2. Created `responsive-image.html` applying `max-width: 100%` and `height: auto` to scale an image smoothly inside narrow windows.
3. Created `responsive-text.html` setting base body text to `1rem` and scaling `h1` heading from `1.5rem` to `2.5rem` via `@media (min-width: 600px)`.
4. Captured and verified browser output screenshots for all tasks into `lab-15/images/`.

## 5. Command Log / Source Code

### Task 1: `mobile-first.html`
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mobile First Responsive Layout</title>
    <style>
        body { font-family: Arial, sans-serif; padding: 20px; margin: 0; }
        .cards { display: flex; flex-direction: column; gap: 15px; }
        .card { background-color: #f4f4f4; border: 1px solid #ddd; padding: 20px; border-radius: 8px; }
        @media (min-width: 600px) {
            .cards { flex-direction: row; }
            .card { flex: 1; }
        }
    </style>
</head>
<body>
    <h1>Mobile-First Cards</h1>
    <div class="cards">
        <div class="card">
            <h2>Card One</h2>
            <p>This is the first card content that stacks on small screens and sits side-by-side on larger screens.</p>
        </div>
        <div class="card">
            <h2>Card Two</h2>
            <p>This is the second card content designed using a mobile-first media query layout.</p>
        </div>
    </div>
</body>
</html>


Task 2: responsive-image.html
HTML


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Image</title>
    <style>
        body { font-family: Arial, sans-serif; padding: 20px; }
        img { max-width: 100%; height: auto; border-radius: 8px; }
    </style>
</head>
<body>
    <h1>Responsive Image Scaling</h1>
    <img src="images/sample.jpg" alt="Responsive Sample Photo">
</body>
</html>
Task 3: responsive-text.html
HTML


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Typography</title>
    <style>
        body { font-size: 1rem; font-family: Arial, sans-serif; padding: 20px; }
        h1 { font-size: 1.5rem; color: #1d3557; }
        @media (min-width: 600px) {
            h1 { font-size: 2.5rem; }
        }
    </style>
</head>
<body>
    <h1>Dynamic Responsive Heading</h1>
    <p>This paragraph has a base font size of 1rem. Resize the browser window above 600px to see the h1 heading scale up from 1.5rem to 2.5rem.</p>
</body>
</html>
6. Screenshots & Output Evidence
Task 1 Output: ![Task 1 Mobile First](images/task1.png)   
Screenshot 2026-11-04 195132.png

Task 2 Output: ![Task 2 Responsive Image](images/task2.png)   
Screenshot 2026-11-04 195132.png

Task 3 Output: ![Task 3 Responsive Text](images/task3.png)   
Screenshot 2026-11-04 195132.png

7. Key Learning Outcomes
Mastered mobile-first media query styling patterns using min-width breakpoints.   
Screenshot 2026-11-04 195132.png

Understood how to prevent image overflow using relative percentage width bounds.   
Screenshot 2026-11-04 195132.png

Applied scalable typography practices using rem units in responsive contexts[cite: 14].

8. Common Errors & Troubleshooting
Missing Viewport Tag: Omitting <meta name="viewport" content="width=device-width, initial-scale=1.0"> prevents mobile devices from rendering media queries accurately[cite: 14]. Ensured inclusion in <head>.

9. Viva / Interview Questions
Q: Why is the viewport meta tag necessary for responsive web design?

A: It tells the browser to set the page width to the screen width of the device and initializes the scale level[cite: 14].

Q: What is the difference between max-width: 100% and width: 100% on images?

A: max-width: 100% allows images to shrink on smaller screens while preventing them from stretching larger than their original size[cite: 14]. width: 100% forces images to stretch to full container width regardless of original dimensions.

10. Submission Checklist
[x] Task 1 (mobile-first.html) code & screenshot[cite: 14]

[x] Task 2 (responsive-image.html) code & screenshot[cite: 14]

[x] Task 3 (responsive-text.html) code & screenshot[cite: 14]

[x] Complete README documentation
