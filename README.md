# Ex.08 Design of Interactive Image Gallery
# Date:6.12.2024
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```

html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gallery</title>
    <style>
        #flexbox
        {
            /* border: 5px solid pink; */
            padding: 170px;
            background-image: url("images.jpeg");
            background-repeat: no-repeat;
            background-size: cover;
        }
        #container1
        {
            /* margin-left:25%; */
            display: flex;
            background-color: whitesmoke; 
            gap: 20px;
            justify-content: center;
            padding: 20px;
            box-shadow: 0 2px 3px;
        }
        #container2
        {
            gap: 20px;
            display: flex;
            background-color: whitesmoke; 
            justify-content: center;
            /* border: 5px inset black; */
            padding: 10px;
            box-shadow:0 2px 3px;
        }
        .img
        {
            height: 190px;
            width: 260px;
            /* transform: rotate(-10deg); */
            image-rendering:optimizeQuality;    
            border: 2px inset whitesmoke;    
            border-radius: 10px;
            box-shadow:  0 0 10px black ;
            transition: 0.5s;
        }
        .img:hover
        {
            content: 'hello';
            transform: scale(1.3);
        }
        #divs
        {
            display: inline;
        }
        #image
        {
            z-index: 100;
            display: none;
            background: rgba(0,0,0,0.5);
            position: fixed;
            width: 100%;
            /* transform: rotate(20deg); */
            height: 100%;
            top: 0;
            bottom: 0;
            align-items: center;
            justify-content: center;    
        }
        #image img{
            width: 600px;
            height: auto;
        }
        #title
        {
            background-color: white;
            border-radius: 10px;
            width: 500px;
            box-shadow: 0 3px 10px;
            position: absolute;
            top: 20px;
            left: 500px;
        }
    </style>
</head>
<body>
    <section id="image">
            <img src="C:\Users\admin\Desktop\images.jpeg" alt="" id="display" onclick="closes()">
    </section>
<div id="flexbox">

    <h1 align="center" style="color: black;"><span id="title">SUPER CARS </span></h1>

    <div id="container1">
        <div class="divs"><img class="img" src="car1.jpg" onclick="opens(this.src)" alt=""></div>
        <div class="divs"><img class="img" src="car2.jpg" onclick="opens(this.src)"   alt=""></div>
        <div class="divs"><img class="img" src="car5.avif"  onclick="opens(this.src)"  alt=""></div>
        <div class="divs" ><img class="img" src="car0.jpg" onclick="opens(this.src)"   alt=""></div>
    </div>
    <div id="container2">
        <div class="divs" ><img class="img" src="car6.jpg" onclick="opens(this.src)"  alt=""></div>
        <div class="divs"><img class="img" src="car7.jpg" onclick="opens(this.src)"  alt=""></div>
        <div class="divs" ><img class="img" src="car8.jpg" onclick="opens(this.src)"  alt=""></div>
       <div class="divs"><img class="img" src="car9.jpeg" onclick="opens(this.src)"  alt=""> </div>
    </div>
    
</div>
<footer align="center" style="background-color:black">
    <p>Designed & Developed by Santhosh Venkatesan &copy; </p>
</footer>
    <script>
            var a =document.getElementById("image");
            var b=document.getElementById("display");
            function opens(c)
            {
                a.style.display='flex';
                b.src=c;
            }
            function closes()
            {
                a.style.display='none';
            }
    </script>
</body>
</html>

  ```
# OUTPUT:


![Screenshot 2024-12-16 021013](https://github.com/user-attachments/assets/4714207c-54ad-4a6b-b44a-170078cf5490)
![Screenshot 2024-12-16 021427](https://github.com/user-attachments/assets/4f0121d5-71e4-4c1f-a54c-d39ec79e2d80)

![Screenshot 2024-12-16 021528](https://github.com/user-attachments/assets/79008c35-bb9a-440b-8c2d-e97124e7e555)

![Screenshot 2024-12-16 021501](https://github.com/user-attachments/assets/ca2e7cc0-67c3-4ac2-90c6-06a848155d27)

![Screenshot 2024-12-16 021546](https://github.com/user-attachments/assets/ce4c91d7-61af-4ec0-8541-0a0457fc80b3)

# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
