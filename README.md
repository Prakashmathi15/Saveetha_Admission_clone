# Saveetha_Admission_clone
## Date: 9/07/25

## Objective:
To design a landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS. This activity reinforces skills in layout design, form creation, user input handling, responsive structure, and visual styling based on a real-world example.

## Tasks:
#### 1. Analyze the Landing Page Layout:
Observe the split-screen layout with a promotional section on the left and a form on the right.

Note the use of background images, text styling, and branding elements.

#### 2. Create the HTML Structure:
Use semantic tags like ```<section>, <header>, <form>, and <footer>``` to organize content.

Structure the form with input fields such as name, email, phone, password, city, state, course, specialization, captcha, and checkbox.

#### 3. Add Form Functionality:
Include appropriate input types (text, email, tel, password, select, etc.) with placeholders and labels.

Use the <button> element for the "APPLY NOW" action.

#### 4. Apply CSS Styling:
Implement a split layout using flexbox or grid.

Style the form elements with padding, shadows, background colors, and rounded borders.

Include hover effects and button transitions to match the original look.

#### 5. Incorporate Images and Branding:
Add the institution logo and use matching fonts and colors.

Place a background image or blurred overlay behind the form content if needed.

#### 6. Ensure Responsiveness:
Make sure the page adapts to different screen sizes using media queries.

Maintain readability and layout integrity on both desktop and mobile.

## HTML Code:
```html
<!DOCTYPE html>
<html lang="en">
<head>
 
  <title>Saveetha Admission Enquiry</title>
  <link rel="stylesheet" href="style.css">
 
</head>
<body>
  <div class="container">
    <section class="left-panel">
      <img src="logo.png" alt="Saveetha Logo" class="logo">
      <p class="tnea-code">TNEA CODE <span>1216</span></p>
      <h1 class="headline">INDUSTRY 5.0</h1>
      <p class="subtext">Ready Curriculum Imparting <br><strong>21st Century Skills</strong></p>
      <button class="apply-btn">Apply Now ▼</button>
    </section>

    <section class="right-panel">
      <form class="admission-form">
        <h2>Admissions Open 2025</h2>
        
        <input type="text" placeholder="Enter Name *" required>
        <input type="email" placeholder="Enter Email Address *" required>
        <input type="tel" placeholder="Enter Mobile Number *" required>
        <input type="password" placeholder="Any Password of Your Choice *" required>

        <div class="row">
          <select required>
            <option value="">State *</option>
            <option value="Tamil Nadu">Tamil Nadu</option>
            <option value="Karnataka">Karnataka</option>
          </select>
          <input type="text" placeholder="City *" required>
        </div>

        <div class="row">
          <select required>
            <option value="">Course *</option>
            <option value="B.Tech">B.Tech</option>
            <option value="B.E">B.E</option>  

          </select>
          <input type="text" placeholder="Specialization *" required>
        </div>

        <div class="captcha">
          <img src="captcha.jpeg" alt="Captcha">
          <input type="text" placeholder="Enter text as shown" required>
        </div>

     <div class="checkbox-group">
    <label class="checkbox-label">
    <input type="checkbox" required>
    <span>I authorise American Baptist College...</span>
    </label>
    </div>


        <button type="submit" class="submit-btn">APPLY NOW ▶</button>
        <p class="login-text">Already have an Account? <a href="#">Login</a> | <a href="#">Resend Verification Email</a></p>
      </form>
    </section>
  </div>
</body>
</html>


```

## CSS Code:
```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}

body {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background: #f5f5f5;
}

.container {
  display: flex;
  width: 100%;
  height: 100vh;
}

.left-panel {
  flex: 1;
  background: url('college.jpg') no-repeat center center/cover;
  color: rgb(241, 231, 231);
  padding: 100px;
  position: relative;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.logo {
  width: 175px;
}

.tnea-code {
  margin-top: 20px;
  font-weight: bold;
  font-size: 18px;
}

.headline {
  font-size: 48px;
  font-weight: bold;
  margin-top: 30px;
  color: #02fb4d;
}

.subtext {
  margin-top: 20px;
  font-size: 20px;
}

.apply-btn {
  margin-top: 30px;
  padding: 12px 24px;
  background: #ffd700;
  color: black;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-weight: 600;
}

.right-panel {
  flex: 1;
  background: rgba(255, 255, 255, 0.95);
  padding: 1px;
  display: flex;
  justify-content: center;
  align-items: center;
    position: relative;
}

.admission-form {
  width: 100%;
  max-width: 400px;
}

.admission-form h2 {
  margin-bottom: 20px;
  font-weight: 600;
}

.admission-form input,
.admission-form select {
  width: 100%;
  padding: 10px;
  margin-bottom: 15px;
  border: 1px solid #ccc;
  border-radius: 6px;
}

.row {
  display: flex;
  gap: 10px;
}

.captcha {
  display: flex;
  align-items: center;
  gap: 10px;
  
}
.captcha img {
  width: 100px;
  height: 40px;
  border: 1px solid #ccc;
  border-radius: 6px;
}

.checkbox-label {
  display: flex;
  align-items: center;
  font-size: 14px;
  color: #333;
  line-height: 1.4;
}






.submit-btn {
  margin-top: 20px;
  background: #f4b431;
  color: #000;
  padding: 12px;
  width: 100%;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  font-weight: 600;
  transition: background 0.3s;
}

.submit-btn:hover {
  background: #07e120;
}

.login-text {
  margin-top: 15px;
  font-size: 13px;
}

.login-text a {
  color: #007bff;
  text-decoration: none;
}

```

## Output:
<img width="953" alt="image" src="https://github.com/user-attachments/assets/8fd8f117-3a35-4124-a67b-52c9969f87a8" />


## Result:
A landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS is designed successfully.
