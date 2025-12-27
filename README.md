# Ex08 Event Registration Web Application
## Date:27-12-2025

## AIM:
To design, develop and deploy a web application for event registration using Figma UI tool.

## UI DESIGN TOOL:
Figma

## DESIGN STEPS:

### Step 1:
Use frames to represent screens or sections.

### Step 2:
Add column grids for consistent spacing and alignment.

### Step 3:
Insert shapes, text, buttons, and icons.

### Step 4:
Use Auto Layout for flexible, responsive design.

### Step 5:
Define color, text, and effect styles globally for consistency.

### Step 6:
Name layers logically and group related elements.

### Step 6:
Link frames to show navigation or interactions.

### Step 7:
Select the specific frame while generating code using Anima plugin.

## CODE:
Page 1
```
index.html
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="android-medium">
      <img class="sec" src="img/sec-1.png" />
      <p class="dance-fever"><span class="text-wrapper">&nbsp;&nbsp; </span> <span class="span">Dance Fever</span></p>
      <div class="rectangle"></div>
      <div class="ellipse"></div>
      <div class="div">Login</div>
      <div class="register">Register</div>
    </div>
  </body>
</html>
global.css
@import url("https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css");
* {
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
html,
body {
  margin: 0px;
  height: 100%;
}
/* a blue color as a generic focus style */
button:focus-visible {
  outline: 2px solid #4a90e2 !important;
  outline: -webkit-focus-ring-color auto 5px !important;
}
a {
  text-decoration: none;
}
style.css
.android-medium {
  background-color: #8ee2db;
  width: 100%;
  min-width: 700px;
  min-height: 840px;
  position: relative;
}

.android-medium .sec {
  position: absolute;
  top: 19px;
  left: 30px;
  width: 614px;
  height: 150px;
  aspect-ratio: 4.09;
  object-fit: cover;
}

.android-medium .dance-fever {
  position: absolute;
  top: 189px;
  left: 109px;
  width: 485px;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: transparent;
  font-size: 64px;
  letter-spacing: 0;
  line-height: normal;
}

.android-medium .text-wrapper {
  color: #ffffff;
}

.android-medium .span {
  font-family: "JejuHallasan-Regular", Helvetica;
  color: #f40606;
}

.android-medium .rectangle {
  position: absolute;
  top: 357px;
  left: 214px;
  width: 275px;
  height: 125px;
  background-color: #014311;
}

.android-medium .ellipse {
  position: absolute;
  top: 593px;
  left: 216px;
  width: 282px;
  height: 122px;
  background-color: #2b5721;
  border-radius: 141px / 61px;
}

.android-medium .div {
  position: absolute;
  top: 390px;
  left: 262px;
  width: 186px;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #ffffff;
  font-size: 64px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.android-medium .register {
  position: absolute;
  top: 622px;
  left: 287px;
  width: 153px;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #ffffff;
  font-size: 36px;
  letter-spacing: 0;
  line-height: normal;
}
```
PAGE 2
```
index.html
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="android-medium">
      <img class="dance" src="img/dance-1.png" />
      <p class="EVENTS-solo-dance">
        <span class="text-wrapper"
          >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
          <br /><br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
        </span>
        <span class="span">EVENTS</span>
        <span class="text-wrapper">
          <br />
          <br />⭐ Solo Dance <br />⭐ Duo Dance <br />⭐ Group Dance <br />⭐ Classical Dance <br />⭐ Folk Dance
          <br />⭐ Western Dance <br />⭐ Freestyle Dance <br />⭐ Fusion Dance</span
        >
      </p>
    </div>
  </body>
</html>
global.css
@import url("https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css");
* {
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
html,
body {
  margin: 0px;
  height: 100%;
}
/* a blue color as a generic focus style */
button:focus-visible {
  outline: 2px solid #4a90e2 !important;
  outline: -webkit-focus-ring-color auto 5px !important;
}
a {
  text-decoration: none;
}
style.css
.android-medium {
  background-color: #fefffe;
  width: 100%;
  min-width: 700px;
  min-height: 840px;
  position: relative;
}

.android-medium .dance {
  position: absolute;
  top: 0;
  left: 0;
  width: 700px;
  height: 840px;
  aspect-ratio: 0.67;
  object-fit: cover;
}

.android-medium .EVENTS-solo-dance {
  position: absolute;
  top: 72px;
  left: 57px;
  width: 577px;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #000000;
  font-size: 36px;
  letter-spacing: 0;
  line-height: normal;
}

.android-medium .text-wrapper {
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #000000;
  font-size: 36px;
  letter-spacing: 0;
}

.android-medium .span {
  font-family: "Lemon-Regular", Helvetica;
}
```
PAGE 3
```
index.html
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="android-medium">
      <img class="REG" src="img/REG-1.png" />
      <div class="FOR-REGISTRATION">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; FOR REGISTRATION</div>
      <p class="NAME-DEPT-YEAR-DOB">
        NAME:<br />DEPT:<br />YEAR:<br />DOB:<br />CONTACT:<br />EMAIL:<br />NAME OF THE EVENT:<br />DURATION:<br />NUMBER
        OF PARTICIPANTS:<br />TEAM NAME:
      </p>
    </div>
  </body>
</html>
global.css
@import url("https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css");
* {
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
html,
body {
  margin: 0px;
  height: 100%;
}
/* a blue color as a generic focus style */
button:focus-visible {
  outline: 2px solid #4a90e2 !important;
  outline: -webkit-focus-ring-color auto 5px !important;
}
a {
  text-decoration: none;
}
style.css
.android-medium {
  background-color: #ffffff;
  width: 100%;
  min-width: 688px;
  min-height: 825px;
  position: relative;
}

.android-medium .REG {
  position: absolute;
  top: 0;
  left: 0;
  width: 688px;
  height: 825px;
  aspect-ratio: 0.66;
  object-fit: cover;
}

.android-medium .FOR-REGISTRATION {
  position: absolute;
  top: 51px;
  left: 82px;
  width: 485px;
  font-family: "Inter-BoldItalic", Helvetica;
  font-weight: 700;
  font-style: italic;
  color: #000000;
  font-size: 36px;
  letter-spacing: 0;
  line-height: normal;
}

.android-medium .NAME-DEPT-YEAR-DOB {
  position: absolute;
  top: 185px;
  left: 54px;
  width: 559px;
  font-family: "Inter-BoldItalic", Helvetica;
  font-weight: 700;
  font-style: italic;
  color: #000000;
  font-size: 36px;
  letter-spacing: 0;
  line-height: normal;
}
```

## OUTPUT:
<img width="1920" height="1080" alt="Screenshot (56)" src="https://github.com/user-attachments/assets/23da9ecb-935b-426f-85a8-a923ea095f4f" />

## RESULT:
The program to design, develop and deploy a web application for event registration using Figma UI tool is completed successfully.
