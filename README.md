### EX NO: 05

# <p align="center">Website recreation using vertical Farms using HTML & CSS</P>

## Aim:
To create a responsive web page for a vertical farming startup, with a navigation bar, content section, and information boxes.

## Algorithm:

Step 1: Create an HTML file with the necessary structure and add a CSS

Step 2: Define a container div for the entire webpage.

Step 3: Create a navigation bar with a logo and navigation links.

Step 4: Add buttons for "Start free trial" and "Account".

Step 5: Create a content section with text, images, and buttons
  
Step 6: Include information boxes with accompanying circles.
  
Step 7: Apply appropriate classes and styles to the elements.
  
Step 8: Apply appropriate classes and styles to the elements.
  
Step 9: Reset default margin, padding, and box-sizing.
  
Step 10: Style the navigation bar, heading, and navigation links.
  
Step 11: Apply styles to the buttons and arrow icon.
  
Step 12: Set up the row and column layout for the content section.
  
Step 13:  Style the text, images, and information boxes.
  
Step 14: . Test the webpage to ensure proper display and functionality.


## Program

### index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="assests/css/style.css"><link rel="preconnect" href="https://fonts.googleapis.com">
    
    <title>Vertical Farming</title> 
</head>
<body>
    <nav>
        <ul>
        <li><img class="Logo" src="assests/images/Logo.png"></li>
        <li><h2 class="Logotitle">Vertical Farm</h2></li>
        </ul>
        <ul>
            <li style="color: rgb(253, 251, 165);">Solutions</li>
            <li>Department</li>
            <li>Farming Method</li>
            <li>Company</li>
            <li>About</li>
        </ul>
        <ul><button class="FreeTrial">Start Free Trail</button>
        <button class="Account">Account</button>
        </ul>
    </nav>

    <section>
        <p class="heading">
            Fresh, Sustainable,</br>
            Plant <span style="font-weight: bold;">Grow vertically</span></br>
            in <span style="font-weight: bold; background-color: rgb(248, 248, 159); color: black; ">Urban Areas</span>
        </p>
        
        <p class="para">
            Our vertical farming startup brings sustainable, locally grown produce to</br>
            urban areas. With our innovative technology, we're revolutionizing the way</br>
            we grown and consume fresh food.
        </p>
        <button class="startnow">Start Now</button>
        <button class="howItWorks">HOW IT WORKS?</button>
        <img class="Plant1" src="assests/images/plant1.jpg">
        <img class="Plant2" src="assests/images/plant2.jpg">
        <img class="Plant3" src="assests/images/plant3.jpg">
        <br><br>
        <br><br>
        <button class="BoxOne">
            <span class="NumberOne">1</span>
            <span class="BoxOneHeading">Choose the right crops</span><br>
            <span class="BoxOnePara">Select the best crops for your vertical forming</span>
        </button>
        <button class="BoxTwo">
            <span class="NumberTwo">2</span>
            <span class="BoxTwoHeading">Set up grow system</span><br>
            <span class="BoxTwoPara">Install and set up your vertical grow system</span>
        </button>
        <button class="BoxThree">
            <span class="NumberThree">3</span>
            <span class="BoxThreeHeading">Monitor crops</span><br>
            <span class="BoxThreePara">Regularly monitor your crops</span>
        </button>

    </section>

    <footer>
        <button class="StartAt">Farm Start At  <span class="time">7 AM</span></button>
        <img class="Leaf" src="assests/images/footerleaf.png" alt="">
        <span class="footerpara">We offer Consulting Services For Vertical Farming Method </span>
        <ul>
            <button class="DontWait">Don't wait</button>
            <button class="JoinUs">Join us</button>
            <button class="ActNow">Act now</button>
        </ul>
        <ul>
            <button class="ContactTeam">Contact Team</button>
        </ul>
        <img class="icon1" src="assests/images/people1.jpeg"/>
        <img class="icon2" src="assests/images/people2.png"/>
        <img class="icon3" src="assests/images/people3.png"/>
    </footer>
</body>
</html>


```

### style.css
```css
*{
	background-color: black;
	font-family: 'Montserrat', sans-serif;
	color: white;
  }
  .Logo{
	width: 80%;
	height: 80%;
	position: relative;
	left:10px;
	
  }
  .Logotitle{
	font-size: 220%;
	font-weight: 100;
	margin: 0 0;
	position: relative;
	top:-16px;
	left:-20px;
  }
  nav{
	display: flex;
	align-items: center;
	justify-content: space-between;
  
  }
  nav ul li{
	list-style: none;
	display: inline-block;
	color: white;
	padding: 10px 10px;
	font-size: 80%;
	position: relative;
	right: 40px;
  }
  .FreeTrial{
	width: 10.5em;
	height: 3em;
	border-radius: 30em;
	font-size: 13px;
	font-weight: 300;
	font-family: inherit;
	background-color: #000000;
	color: #f1ffa2;
	border: solid 1px #f1ffa2;
	position: relative;
	right: 30px;
	z-index: 1;
  }
  .Account{
	margin: 10px;
	width: 95px;
	height: 40px;
	border-radius: 30em;
	font-size: 13px;
	font-weight: 600;
	font-family: inherit;
	background-color: #f1ffa2;
	color: black;
	border: none;
	position: relative;
	right: 30px;
	z-index: 1;
  }
  section{
	margin: 6%;
	margin-top: -2%;
  }
  .heading{
	font-size: 350%;
	width:60%;
	line-height: 1.0;
  }
  
  section i{
	color: rgb(136, 255, 136);
  }
  
  .para{
	font-size: 15px;
	width: 52%;
  }
  section img{
	width: 45px;
	height: 45px;
	border-radius: 50px;
	position: relative;
	border: solid 1.5px black;
	top:20px;
  }
  .Plant1{
	z-index: 0;
	left: 50px;
  
  }
  .Plant2{
	z-index: 1;
	left: 35px;
  
  }
  .Plant3{
	z-index: 2;
	left: 20px;
  
  }
  .BoxOne{
	padding-left: 0;
	padding-top: 1% ;
	padding-bottom: 1%;
	padding-right: 17%;
	background-color: #e1f2c1;
	border-radius :15px;
	border: none;
  }
  .NumberOne{
	background-color: #ffffff;
	color: black;
	height: 20%;
	padding: 5% 8%;
	border-radius: 100%;
	border: solid .5px #000000;
	position: relative;
	top:7px;
  }
  .BoxOneHeading{
	background-color: #e1f2c1;
	color: #000000;
	font-size: 90%;
	font-weight: 600;
	position: relative;
	left:4%;
	top:-3px;
  }
  .BoxOnePara{
	background-color: #e1f2c1;
	color: #000000;
	font-size: 70%;
	font-weight: 100;
	position: relative;
	left: 32%;
  }
  .BoxTwo{
	padding-left: 0;
	padding-top: 1% ;
	padding-bottom: 1%;
	padding-right: 10%;
	background-color: #fff99f;
	border-radius :15px;
	border: none;
  }
  .NumberTwo{
	background-color: #000000;
	color: rgb(255, 255, 255);
	height: 20%;
	padding: 5% 8%;
	border-radius: 100%;
	border: solid .5px #000000;
	position: relative;
	top:7px;
  }
  .BoxTwoHeading{
	background-color: #fff99f;
	color: #000000;
	font-size: 90%;
	font-weight: 600;
	position: relative;
	left:4%;
	top:-3px;
  }
  .BoxTwoPara{
	background-color: #fff99f;
	color: #000000;
	font-size: 70%;
	font-weight: 100;
	position: relative;
	left: 32%;
  }
  .BoxThree{
	padding-left: 0%;
	padding-top: 1% ;
	padding-bottom: 1%;
	padding-right: 10%;
	background-color: #ffffd3;
	border-radius :15px;
	border: none;
  }
  .NumberThree{
	background-color: #000000;
	color: rgb(251, 250, 250);
	height: 20%;
	padding: 5% 8%;
	border-radius: 100%;
	border: solid .5px #000000;
	position: relative;
	top:7px;
  }
  .BoxThreeHeading{
	background-color: #ffffd3;
	color: #000000;
	font-size: 90%;
	font-weight: 600;
	position: relative;
	left:4%;
	top:-3px;
  }
  .BoxThreePara{
	background-color: #ffffd3;
	color: #000000;
	font-size: 70%;
	font-weight: 100;
	position: relative;
	left: 32%;
  }
  .startnow{
	width: 9em;
	height: 3em;
	border-radius: 30em;
	font-size: 13px;
	font-weight: 600;
	font-family: inherit;
	background-color: #f1ffa2;
	color: black;
	border: none;
	position: relative;
	overflow: hidden;
	z-index: 1;
  }
  .howItWorks{
	margin: 10px;
	width: 14%;
	height: 3em;
	border-radius: 30em;
	font-size: 13px;
	font-weight: 200;
	font-family: inherit;
	background-color: #000000;
	color: #e1f2c1;
	border: solid 1px #e1f2c1;
	position: relative;
	overflow: hidden;
	z-index: 1;
	
   }
  
  footer{
	height: 140px;
	display: flex;
	align-items: center;
	justify-content: space-between;
	color:black;
	background-color: white;
	
  
  }
  .StartAt{
	width:13em;
	height: 4em;
	font-size: 12px;
	font-weight: 300;
	letter-spacing: -0.1px;
	background-color: #000000;
	color: rgb(255, 255, 255);
	border: solid 1px black;
	position: relative;
	left: 75px;
  }
  .time{
	padding: 6px 6px;
	border-radius: 90px;
	font-size: 10px;
	background-color: #ffffff;
	color: rgb(0, 0, 0);
	font-weight: 600;
	position: relative;
	left: 3px;
  }
  .Leaf{
	position: relative;
	left: 33px;
	height: 48px;
	width: 48px;
  }
  
  footer ul{
	background-color: white;
  }
  footer ul li{
	list-style: none;
	display: inline-block;
	color: white;
	padding: 10px 10px;
	background-color: white;
  }
  .footerpara{
	width: 22%;
	margin-left: 100px;
	font-size:18px;
	color:black;
	background-color: white;
	font-weight: 600;
  }
  
  footer button{
	width: 110px;
	height: 40px;
	border-radius: 30em;
	font-size: 11px;
	font-weight: 600;
	font-family: inherit;
	background-color: #f1ffa2;
	color: black;
	border: solid 1px black;
  }
  .DontWait{
	position: relative;
	z-index: 2;
	
  
  }
  .JoinUs{
	background-color: #e5e8fe;
	margin: -40px;
	/* z-index:4; */
	padding-right:0px;
	padding-left:14%;
	position: relative;
	z-index: 1;
	left:-10px;
  }
  .ActNow{
	background-color: #fcecbe;
	/* z-index: 2; */
	padding-left: 9%;
	padding-right: 0px;
	position: relative;
	z-index:0;
	left:-10px;
  }
  .ContactTeam{
	width: 130px;
	height: 40px;
	border-radius: 30em;
	font-size: 12px;
	font-weight: 500;
	background-color: #ffffff;
	color: rgb(0, 0, 0);
	border: solid 1px rgb(0, 0, 0);
	position: relative;
	overflow: hidden;
	z-index: 1;
  }
  footer img{
	width: 35px;
	height: 35px;
	border-radius: 50px;
	position: relative;
	border: solid 1px black;
	object-fit: cover;
  }
  .icon1{
	z-index: 2;
   left: 50px;
  
  }
  .icon2{
	z-index: 1;
	left:1px;
  
  }
  .icon3{
	z-index: 0;
	left: -50px;
  
  }
  

```

## Output

![Screenshot 2023-06-04 120359](https://github.com/Gowri4622/html-farm/assets/75235455/50672169-a061-4975-b3cb-cddecd5e1a0c)



## Result
Thus we Successfully Re created the given snap of the website using HTML & CSS
  
