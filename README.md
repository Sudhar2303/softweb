# Ex.07 Software Product Company Website
## DATE: 31/10/2023
## AIM:
To develop a static company website to display the softwares and services provided by the company.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
### sample.html:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Webpage Design</title>
    <link rel="stylesheet" href="style.css">
    <script src="script.js"></script>
</head>
<body>

    <div class="main">
        <div class="navbar">
            <div class="icon">
                <h2 class="logo">Software Solutions</h2>
            </div>
            <h2 style = " font-family: Monotype Corsiva, sans-serif;float: right; color: aliceblue; padding: 20px;">login/signup</h2>
            <div class = "container">
                <nav>
                    <ul>
                        <li onclick="showContent('Home')">Home</li>
                        <li onclick="showContent('products')">products</li>
                        <li onclick="showContent('People')">People</li>
                        <li onclick="showContent('ContactUs')">ContactUs</li>
                    </ul>
                 </nav>
            </div>
        </div> 
        <section id="Home" class="active">
            <div class = "center"> 
                <div class ="white-box">
                    <div class = "line">
                        <img src = "slide6.jpg" style="width: 600px; height: 300px; padding-top: 50px; padding-left: 20px;">
                        <h2 style ="font-size: 30; font-family: Gabriola; padding: 20px; padding-top: 80px;">Empowering Tomorrow, Today: Seamless Solutions for a Digital Universe</h2>
                    </div>
                </div>
                <h2 style ="font-size: 70; font-family: Gabriola; padding-left: 230px;color: rgb(255, 255, 255);">"Beyond Solutions, We Deliver Experiences: Your Vision, Our Expertise, Unleashing Possibilities."</h2>
            </div>
        </section>
        <section id="products">
            <div class = "center">
                <div class = "white-box">
                    <img src = "360_F_444957775_JoCfyM0odoSzyM8bimtz9T2FAyQVfiMZ.jpg" style="width: 1000px; height: 300px; padding-top: 50px; padding-left: 30px;">
                </div>
                <h2 style ="font-size: 70; font-family: Gabriola; padding-left: 300px;color: aliceblue;">"Tailored Solutions, Diverse Products: Servicing Success in Every Sector."</h2>
            </div>
        </section>
        <section id="People">
            <div class = "center">
                <div class = "white-box">
                    <div class = "line">
                        <img src = "06.jpg"  alt="Avatar" style="width: 140px; height: 160px; padding: 40px;border-radius: 50%;">
                        <img src = "01.jpg" alt="Avatar" style="width: 140px; height: 160px;padding: 40px;border-radius: 50%;">
                        <img src = "02.jpg" alt="Avatar" style="width: 140px; height: 160px;padding: 40px;border-radius: 50%;">
                        <img src = "03.jpg" alt="Avatar" style="width: 140px; height: 160px;padding: 40px;border-radius: 50%;">
                        <img src = "04.jpg" alt="Avatar" style="width: 140px; height: 160px;padding: 40px;border-radius: 50%;">
                    </div>
                    <div class = "line">
                        <h4 style ="font-family: Times New Roman; padding-left: 25px;color: rgb(0, 0, 0);">SUDHARSANAN V (COO)</h4>
                        <h4 style ="font-family: Times New Roman; padding-left: 30px;color: rgb(0, 0, 0);">MANIKANDAN P (CEO)</h4>
                        <h4 style ="font-family: Times New Roman; padding-left: 40px;color: rgb(0, 0, 0);">AISHWARIYA T M (HR)</h4>
                        <h4 style ="font-family: Times New Roman; padding-left: 75px;color: rgb(0, 0, 0);">MAHESH S (MD)</h4>
                        <h4 style ="font-family: Times New Roman; padding-left: 90px;color: rgb(0, 0, 0);">KAUSHIK R (CFO)</h4>
                    </div>
                </div>
                
            </div>
        </section>
        <section id="ContactUs">
            <div class = "center">
                <div class = "white-box">
                    `<div class="contact-form">
                        <h1>Contact Us</h1>
                        <form action="submit_form.php" method="POST">
                            <div class="form-group">
                                <input type="text" id="name" name="name" placeholder="Your Name" required>
                            </div>
                            <div class="form-group">
                                <input type="email" id="email" name="email" placeholder="Your Email" required>
                            </div>
                            <div class="form-group">
                                <textarea id="message" name="message" placeholder="Your Message" rows="5" required></textarea>
                            </div>
                            <button type="submit">Submit</button>
                        </form>
                    </div>  
                </div>
            </div>
        </section>
    </div>
</body>
</html>
```
### style.css:
```
style.css
*{
    margin: 0;
    padding: 0;
}

.main
{
    width: 100%;
    background: linear-gradient(to top, rgb(0, 0, 0)0%,rgb(0, 0, 0)30%);
    background-position: center;
    background-size: cover;
    height: 100vh;
}

.navbar{
    width: 1200px;
    height: 75px;
    margin: auto;
}

.icon{
    width: 200px;
    float: left;
    height: 70px;
}

.logo{
    color: #5500dd;
    font-size: 35px;
    font-family: Arial;
    padding-left: 20px;
    float: left;
    padding-top: 10px;
    margin-top: 5px
}

.menu{
    width: 400px;
    float: left;
    height: 70px;
}
nav
{
  padding: 30px 300px;
}
nav ul li
{
  list-style: none;   
  display: inline-table;
  padding: 0px 23px;
  margin: 3px;
  font-size: 18px;
  font-weight: 500;
  color: #777;
  cursor: pointer;
  position: relative;
  z-index: 2;
  transition: color 0.5s;
}
nav ul li::after{
  content: '';
  background: #f44566;
  width: 100%;
  height: 100%;
  position: absolute;
  top: 100%;
  left: 50%;
  transform: translate(-50% ,-50%);
  z-index: -1;
  opacity: 0;
  transform: top 0.5s ,opacity 0.5s;
}
nav ul li:hover
{
  color:#fff;   
}
nav ul li:hover::after
{
  top : 50%;
  opacity: 1;
}
.center
{
  padding-left: 100px;
  padding-top: 100px;
}
.white-box
{
  width: 1100px;
  height: 400px;
  background-color: white;
  border: 1px solid #ccc;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

section {
  display: none;
}

section.active {
  display: block;
}
.line
{
  display: flex;
}
.contact-form, .contact-info {
  padding: 20px;
  flex: 1;
}
.contact-form {
  text-align: left;
}
.form-group {
  margin: 10px 0;
}
input[type="text"],
input[type="email"],
textarea {
    width: 50%;
    padding: 10px;
    margin: 5px 0;
    border: 1px solid #ccc;
    border-radius: 5px;
}
```
### script.js:
```
function showContent(option) 
{
    const plantsContentDiv = document.getElementById('Home');
    const seedsContentDiv = document.getElementById('products');
    const planterContentDiv = document.getElementById('People');
    const soilContentDiv = document.getElementById('ContactUs');

    if (option === 'Home') {
        plantsContentDiv.style.display = 'block';
        seedsContentDiv.style.display = 'none';
        planterContentDiv.style.display = 'none';
        soilContentDiv.style.display = 'none';
        
    }
    else if (option === 'products') {
        plantsContentDiv.style.display = 'none';
        seedsContentDiv.style.display = 'block';
        planterContentDiv.style.display = 'none';
        soilContentDiv.style.display = 'none';
    }
    else if (option === 'People') {
        plantsContentDiv.style.display = 'none';
        seedsContentDiv.style.display = 'none';
        planterContentDiv.style.display = 'block';
        soilContentDiv.style.display = 'none';
    }
    else if (option === 'ContactUs') {
        plantsContentDiv.style.display = 'none';
        seedsContentDiv.style.display = 'none';
        planterContentDiv.style.display = 'none';
        soilContentDiv.style.display = 'block';
    }
}
```
## OUTPUT:
![Alt text](<Screenshot (308).png>)
![Alt text](<Screenshot (309).png>)
![Alt text](<Screenshot (310).png>)
![Alt text](<Screenshot (311).png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
