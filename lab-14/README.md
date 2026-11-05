# Lab 14: CSS Grid Layouts

## 1. Practical Aim
To construct two-dimensional layouts using CSS Grid, including equal fractional columns, responsive photo galleries with `auto-fill` and `minmax()`, and named layout areas using `grid-template-areas`.

## 2. Theoretical Background
- **CSS Grid Layout (`display: grid`):** A powerful 2D grid system for aligning elements in both rows and columns simultaneously.
- **Fraction Unit (`fr`):** Represents a fraction of the available free space in the grid container.
- **Responsive Auto-Fit/Fill (`repeat(auto-fill, minmax(150px, 1fr))`):** Automatically calculates column count based on available screen width while specifying minimum and maximum tile widths.
- **Grid Template Areas (`grid-template-areas`):** Allows naming specific grid cells and assigning elements via `grid-area` to build page layouts.

## 3. Pre-requisites & Tools Used
- Visual Studio Code
- Modern Web Browser (Chrome/Edge)
- Windows File Explorer

## 4. Step-by-Step Procedure
1. Created `grid-first.html` containing six numbered boxes inside a 3-column grid (`repeat(3, 1fr)`) with a 12px gap.
2. Created `gallery.html` featuring a heading "Club Photo Gallery" and six responsive photo containers using `auto-fill` and `minmax(150px, 1fr)`.
3. Created `dashboard-areas.html` defining a grid with 200px sidebar and 1fr main content, mapping full-width header and footer sections using `grid-template-areas`.
4. Captured and verified browser output screenshots for all tasks into `lab-14/images/`.

## 5. Command Log / Source Code

### Task 1: `grid-first.html`
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Grid Equal Columns</title>
    <style>
        .grid-container { display: grid; grid-template-columns: repeat(3, 1fr); gap: 12px; padding: 20px; }
        .box { background-color: #4a90e2; color: white; font-size: 24px; font-weight: bold; display: flex; justify-content: center; align-items: center; height: 100px; border-radius: 6px; }
    </style>
</head>
<body>
    <div class="grid-container">
        <div class="box">1</div><div class="box">2</div><div class="box">3</div>
        <div class="box">4</div><div class="box">5</div><div class="box">6</div>
    </div>
</body>
</html>


Task 2: gallery.html
HTML


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Club Photo Gallery</title>
    <style>
        body { font-family: Arial, sans-serif; padding: 20px; }
        .gallery-container { display: grid; grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)); gap: 10px; margin-top: 20px; }
        .photo-box { background-color: #e0e0e0; border: 2px solid #ccc; height: 120px; display: flex; justify-content: center; align-items: center; font-weight: bold; border-radius: 8px; }
    </style>
</head>
<body>
    <h1>Club Photo Gallery</h1>
    <div class="gallery-container">
        <div class="photo-box">Photo 1</div><div class="photo-box">Photo 2</div><div class="photo-box">Photo 3</div>
        <div class="photo-box">Photo 4</div><div class="photo-box">Photo 5</div><div class="photo-box">Photo 6</div>
    </div>
</body>
</html>
Task 3: dashboard-areas.html
HTML


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dashboard Grid Areas</title>
    <style>
        body { margin: 0; font-family: Arial, sans-serif; }
        .dashboard {
            display: grid;
            grid-template-columns: 200px 1fr;
            grid-template-rows: auto 1fr auto;
            grid-template-areas: 
                "header header"
                "sidebar main"
                "footer footer";
            gap: 10px; min-height: 100vh; padding: 10px; box-sizing: border-box;
        }
        header { grid-area: header; background-color: #333; color: white; padding: 20px; text-align: center; }
        aside { grid-area: sidebar; background-color: #f4f4f4; padding: 20px; border: 1px solid #ddd; }
        main { grid-area: main; background-color: #eef; padding: 20px; border: 1px solid #ccc; }
        footer { grid-area: footer; background-color: #333; color: white; padding: 15px; text-align: center; }
    </style>
</head>
<body>
    <div class="dashboard">
        <header>Dashboard Header</header>
        <aside>Sidebar (200px)</aside>
        <main>Main Content Area (1fr)</main>
        <footer>Dashboard Footer</footer>
    </div>
</body>
</html>
6. Screenshots & Output Evidence
Task 1 Output: ![Task 1 Grid First](images/task1.png)   
Screenshot 2026-11-04 194153.png

Task 2 Output: ![Task 2 Gallery](images/task2.png)   
Screenshot 2026-11-04 194153.png

Task 3 Output: ![Task 3 Dashboard Areas](images/task3.png)   
Screenshot 2026-11-04 194153.png

7. Key Learning Outcomes
Mastered equal-column layout configuration using fr units.

Understood responsive layout behavior using repeat(), auto-fill, and minmax() without media queries[cite: 13].

Learned full page dashboard layout mapping via grid-template-areas[cite: 13].

8. Common Errors & Troubleshooting
Area Mismatch: Spelled area names incorrectly in grid-area vs grid-template-areas. Ensured exact casing and naming syntax.

9. Viva / Interview Questions
Q: What is the difference between auto-fill and auto-fit in CSS Grid?

A: auto-fill creates empty tracks if space allows, whereas auto-fit stretches existing items to fill the extra space.

Q: How does minmax(150px, 1fr) work?

A: It sets the minimum column width to 150px and maximum to 1 fraction of remaining container width[cite: 13].

10. Submission Checklist
[x] Task 1 (grid-first.html) code & screenshot[cite: 13]

[x] Task 2 (gallery.html) code & screenshot[cite: 13]

[x] Task 3 (dashboard-areas.html) code & screenshot[cite: 13]

[x] Complete README documentation

