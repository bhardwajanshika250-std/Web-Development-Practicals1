# Lab 9: Tables with Headers and Footers

## 1. Practical Aim
To construct structured HTML tables with captions, header rows (`<thead>`), body rows (`<tbody>`), footer rows (`<tfoot>`), and accessibility scope attributes (`scope="col"` and `scope="row"`).

## 2. Theoretical Background
- **Table Structure Elements (`<table>`, `<caption>`, `<thead>`, `<tbody>`, `<tfoot>`):** Used to cleanly organize tabular data and semantic sections.
- **Table Cells (`<th>` vs `<td>`):** `<th>` represents header cells (bold and centered by default), while `<td>` represents standard data cells.
- **Scope Attribute (`scope="col"` / `scope="row"`):** Enhances accessibility by explicitly defining whether a header cell relates to a column or a row.

## 3. Pre-requisites & Tools Used
- Visual Studio Code
- Modern Web Browser (Chrome/Edge)
- Windows File Explorer

## 4. Step-by-Step Procedure
1. Created `marks.html` with a table caption (`Marks of Class A`), a header row (`<thead>`), and body rows (`<tbody>`) for Asha, Rohan, and Neha.
2. Created `marks-average.html` containing the same table structure for Asha and Rohan, incorporating a footer (`<tfoot>`) displaying class averages.
3. Created `marks-accessible.html` adding `scope="col"` to header cells and `scope="row"` to name cells for screen reader accessibility.
4. Captured and verified browser output screenshots for all tasks and saved them into `lab-9/images/`.

## 5. Command Log / Source Code

### Task 1: `marks.html`
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Marks of Class A</title>
    <style>
        table, th, td { border: 1px solid black; border-collapse: collapse; padding: 8px; }
    </style>
</head>
<body>
    <table>
        <caption>Marks of Class A</caption>
        <thead>
            <tr>
                <th>Name</th>
                <th>Maths</th>
                <th>Science</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Asha</td>
                <td>78</td>
                <td>85</td>
            </tr>
            <tr>
                <td>Rohan</td>
                <td>64</td>
                <td>70</td>
            </tr>
            <tr>
                <td>Neha</td>
                <td>91</td>
                <td>88</td>
            </tr>
        </tbody>
    </table>
</body>
</html>

Task 2: marks-average.html
HTML


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Marks Average</title>
    <style>
        table, th, td { border: 1px solid black; border-collapse: collapse; padding: 8px; }
    </style>
</head>
<body>
    <table>
        <caption>Marks of Class A</caption>
        <thead>
            <tr>
                <th>Name</th>
                <th>Maths</th>
                <th>Science</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Asha</td>
                <td>78</td>
                <td>85</td>
            </tr>
            <tr>
                <td>Rohan</td>
                <td>64</td>
                <td>70</td>
            </tr>
        </tbody>
        <tfoot>
            <tr>
                <td>Class average</td>
                <td>71</td>
                <td>77.5</td>
            </tr>
        </tfoot>
    </table>
</body>
</html>
Task 3: marks-accessible.html
HTML


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Accessible Marks Table</title>
    <style>
        table, th, td { border: 1px solid black; border-collapse: collapse; padding: 8px; }
    </style>
</head>
<body>
    <table>
        <caption>Marks of Class A</caption>
        <thead>
            <tr>
                <th scope="col">Name</th>
                <th scope="col">Maths</th>
                <th scope="col">Science</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <th scope="row">Asha</th>
                <td>78</td>
                <td>85</td>
            </tr>
            <tr>
                <th scope="row">Rohan</th>
                <td>64</td>
                <td>70</td>
            </tr>
        </tbody>
    </table>
</body>
</html>
6. Screenshots & Output Evidence
Task 1 Output: ![Task 1 Marks](images/task1.png)   
Screenshot 2026-11-04 145703.png

Task 2 Output: ![Task 2 Marks Average](images/task2.png)   
Screenshot 2026-11-04 145703.png

Task 3 Output: ![Task 3 Marks Accessible](images/task3.png)   
Screenshot 2026-11-04 145703.png

7. Key Learning Outcomes
Learned how to organize complex tabular data using <thead>, <tbody>, and <tfoot>.

Understood the importance of table captions for context.

Implemented scope attributes to make tables fully accessible to assistive technologies.

8. Common Errors & Troubleshooting
Border Spacing: Tables appeared unbordered or disconnected by default. Fixed by adding CSS border-collapse: collapse; to table, th, td.

9. Viva / Interview Questions
Q: What is the purpose of the scope attribute in table headers?

A: It explicitly defines whether a header cell applies to a row (scope="row") or a column (scope="col"), helping screen readers navigate data tables[cite: 8].

Q: Where should <tfoot> be placed relative to <tbody> in HTML5?

A: In HTML5, <tfoot> can be placed either before or after <tbody>, provided it is inside the <table> element.

10. Submission Checklist
[x] Task 1 (marks.html) code & screenshot[cite: 8]

[x] Task 2 (marks-average.html) code & screenshot[cite: 8]

[x] Task 3 (marks-accessible.html) code & screenshot[cite: 8]

[x] Complete README documentation


---










