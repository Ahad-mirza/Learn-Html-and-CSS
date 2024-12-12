# 🗓️ Time Table Project

This project creates a **Time Table** web page using HTML. It displays a weekly schedule with subjects for each day, and also includes a "Lunch" section and a "Project" section.

## 🚀 Features
- Displays days of the week (Monday to Friday)
- Lists subjects for each day
- A "Lunch" section with a colspan
- A "Project" section with rowspan

## 📝 Table Structure

The table consists of multiple rows and columns:
1. **Header row**: The table header with the title "TIME TABLE".
2. **Subjects row**: Displays subjects for each day of the week.
3. **Lunch row**: A row merged across all columns for the lunch break.
4. **Project row**: Displays a project section with some cells spanning across multiple rows.

### 🔍 Step-by-step Explanation

1. **Document Structure**
    - The document starts with a `<!DOCTYPE html>` declaration to specify that the page is written in HTML5.
    - The `<html>` tag starts the document, with `lang="en"` to indicate the language is English.

2. **Head Section** 📑
    - The `<head>` section includes metadata:
      - The `<meta charset="UTF-8">` tag ensures proper encoding for special characters.
      - The `<meta name="viewport" content="width=device-width, initial-scale=1.0">` tag ensures the page is responsive and scales well on mobile devices.
      - The `<title>` tag sets the title of the webpage to "table".

3. **Body Section** 🏠
    - Inside the `<body>`, the main content of the page is placed.
    - A `<table>` is used to create the time table structure.

4. **Table Header** 🔤
    - The first row (`<thead><tr>`) contains a header cell (`<th>`) with a `colspan="6"` attribute to merge the header across all 6 columns, with the title "TIME TABLE".

5. **Table Body** 📅
    - The table body (`<tbody>`) consists of multiple rows (`<tr>`).
    - The first row contains the word "HOURS" in the first cell (`<td rowspan="6">`), spanning 6 rows vertically.
    - The remaining cells in this row contain the days of the week (Mon, Tue, Wed, Thu, Fri).

6. **Subject Rows** 📚
    - Each of the next rows (`<tr>`) lists subjects for each day of the week (e.g., "Math", "Science", etc.).

7. **Lunch Row** 🍴
    - The "Lunch" row is created with a `<th colspan="5">` to merge the "Lunch" cell across all columns, making it a separate section.

8. **Project Row** 🖥️
    - The "Project" section has a cell (`<th colspan="2" rowspan="2">`) that spans across two rows and two columns, indicating that the project continues across two time slots.

9. **Closing Tags** ⚙️
    - Finally, all tags are properly closed with `</table>`, `</body>`, and `</html>` to ensure valid HTML structure.

## 🖋️ Code Example

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>table</title>
</head>
<body>

<table>
<thead><tr>
    <th colspan="6">TIME TABLE</th>
    </tr></thead>

<tbody>    
    <tr>
        <td rowspan="6">HOURS</td>
        <td>Mon</td>
        <td>Tue</td>
        <td>Wed</td>
        <td>Thu</td>
        <td>Fri</td>
    </tr>
    <tr>
        <td>Math</td>
        <td>Science</td>
        <td>Math</td>
        <td>Science</td>
        <td>Arts</td>
    </tr>

    <tr>
        <td>Math</td>
        <td>Science</td>
        <td>Math</td>
        <td>Science</td>
        <td>Arts</td>
    </tr>
    <tr>
        <th colspan="5">LUNCH</th>
    </tr>
    <tr>
        <td>Math</td>
        <td>Science</td>
        <td>Math</td>
        <th colspan="2" rowspan="2">project</th>
    </tr>
    <tr>
        <td>Math</td>
        <td>Science</td>
        <td>Math</td>
    </tr>
</tbody>
</table>

</body>
</html>
