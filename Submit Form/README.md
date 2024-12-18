
# Registration Form HTML Tags Explained 🎉

This `README.md` file provides a detailed breakdown of the tags and attributes used in the Registration Form HTML code. Follow along to learn about each tag and its purpose step-by-step! 📝

---

## **1. DOCTYPE Declaration** 📜
```html
<!DOCTYPE html>
```
- Specifies the HTML version (HTML5 in this case).
- Ensures the browser renders the document in standards mode.

---

## **2. `<html>` Tag** 🌐
```html
<html lang="en">
```
- The root element of the HTML document.
- The `lang="en"` attribute specifies the language as English.

---

## **3. `<head>` Tag** 🧠
```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FORM</title>
</head>
```
- Contains meta-information about the document.

### Key Elements:
1. **`<meta charset="UTF-8">`**:
   - Defines character encoding as UTF-8.
2. **`<meta name="viewport">`**:
   - Ensures responsive design for mobile devices.
3. **`<title>`**:
   - Sets the document title as "FORM" (appears in the browser tab).

---

## **4. `<body>` Tag** 🖥️
```html
<body>
    <h2 style="text-align: center;">Registration Form</h3>
```
- Contains the visible content of the page.
- **`<h2>`**: Displays the title "Registration Form" centered using inline CSS.

---

## **5. `<form>` Tag** 📝
```html
<form action="./thank.html" method="get">
```
- Defines the form structure.
- **Attributes**:
  - `action`: Specifies where to send form data (e.g., `thank.html`).
  - `method`: Determines the HTTP method (GET in this case).

---

## **6. `<label>` and `<input>` Tags** 📥
Used for form fields to gather user information.

### Key Fields:
1. **First Name & Last Name**:
   ```html
   <label for="fn">FIRST NAME:</label>
   <input type="text" id="fn" size="20" autofocus placeholder="ABC" required>
   ```
   - **`type="text"`**: Allows text input.
   - **`autofocus`**: Automatically focuses on this field.
   - **`required`**: Makes the field mandatory.

2. **Date of Birth**:
   ```html
   <input type="date" id="db" required>
   ```
   - **`type="date"`**: Provides a date picker.

3. **CNIC**:
   ```html
   <input type="text" id="cn" placeholder="34*****" required>
   ```

4. **Phone**:
   ```html
   <input type="tel" id="tel" value="+92" required>
   ```
   - **`type="tel"`**: Ensures phone number format.
   - **`value`**: Pre-fills with `+92`.

5. **Email**:
   ```html
   <input type="email" id="email" placeholder="xyz@gmail.com" required>
   ```
   - **`type="email"`**: Validates email format.

6. **Password**:
   ```html
   <input type="password" id="ps" placeholder="#123abCD">
   ```
   - **`type="password"`**: Hides input for privacy.

---

## **7. `<select>` Tag** 🎓
```html
<select id="course" name="courses" required>
    <option value="">Graphic Design</option>
    <option value="Web Devolpment">Web Devolpment</option>
    <option value="Video Editing">Video Editing</option>
    <option value="Digital Markiting">Digital Markiting</option>
    <option value="python">Python</option>
</select>
```
- Displays a dropdown menu for course selection.
- **`<option>`**: Represents individual choices.

---

## **8. Gender Selection** 🚻
```html
<label for="M">Male</label>
<input type="radio" name="gender" id="M">
<label for="F">Female</label>
<input type="radio" name="gender" id="F">
<label for="O">Others</label>
<input type="radio" name="gender" id="O">
```
- Uses **`type="radio"`** for single-choice options.

---

## **9. Textarea for Feedback** ✍️
```html
<textarea id="ta" cols="20" rows="5" maxlength="60"></textarea>
```
- Allows users to provide feedback.
- **Attributes**:
  - `cols` and `rows`: Set dimensions.
  - `maxlength`: Limits input to 60 characters.

---

## **10. Checkbox for Agreement** ✅
```html
<label for="ag">I agree to the term of policies</label>
<input type="checkbox" id="ag">
```
- Ensures users agree to terms before submission.

---

## **11. Submit and Reset Buttons** 🛠️
```html
<input type="submit" id="reg">
<input type="reset" id="res">
```
- **`type="submit"`**: Sends the form data.
- **`type="reset"`**: Clears the form.

---

### **🌟 Bonus Tips!**
- Use consistent formatting and indentation.
- Test the form thoroughly to ensure functionality.

Enjoy crafting your HTML forms! 🚀
