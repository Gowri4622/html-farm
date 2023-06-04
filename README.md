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
<html>
<head>
	<title>Shopping Cart UI</title>
	<link rel="stylesheet" href="assets/css/style.css">
	<link href="https://fonts.googleapis.com/css?family=Open+Sans:300,400,600,700,900" rel="stylesheet">
</head>
<body>
   <div class="CartContainer">
   	   <div class="Header">
   	   	<h3 class="Heading">Shopping Cart</h3>
   	   	<h5 class="Action">Remove all</h5>
   	   </div>

   	   <div class="Cart-Items">
   	   	  <div class="image-box">
   	   	  	<img src="assets\img\coffee.jfif"  />
   	   	  </div>
   	   	  <div class="about">
   	   	  	<h1 class="title">Coffee Beans</h1>
   	   	  	<h3 class="subtitle">250gm</h3>
   	   	  	<img src="assets/img/veg.png" />
   	   	  </div>
   	   	  <div class="counter">
   	   	  	<div class="btn">+</div>
   	   	  	<div class="count">1</div>
   	   	  	<div class="btn">-</div>
   	   	  </div>
   	   	  <div class="prices">
   	   	  	<div class="amount">Rs.200/-</div>
   	   	  	<div class="save"><u>Save for later</u></div>
   	   	  	<div class="remove"><u>Remove</u></div>
   	   	  </div>
   	   </div>

   	   
   	 <hr> 
   	 <div class="checkout">
   	 <div class="total">
   	 	<div>
   	 		<div class="Subtotal">Sub-Total</div>
   	 		<div class="items">1 item</div>
   	 	</div>
   	 	<div class="total-amount">Rs.200/-</div>
   	 </div>
    <h2 class="modeofpayment">Mode Of Payment</h2>
    <input type="radio" id="payment" name="mode" value="Online"/> Online <br/> 
   	 <button class="button">Make a Payment</button></div>
   </div>
</body>
</html>


```

### style.css
```css
body{
	margin: 0;
	padding: 0;
	background: linear-gradient(to bottom right, #E3F0FF, #FAFCFF);
	height: 100vh;
	display: flex;
	justify-content: center;
	align-items: center;
}

.CartContainer{
	width: 70%;
	height: 90%;
	background-color: #ffffff;
    border-radius: 20px;
    box-shadow: 0px 10px 20px #1687d933;
}

.Header{
	margin: auto;
	width: 90%;
	height: 15%;
	display: flex;
	justify-content: space-between;
	align-items: center;
}

.Heading{
	font-size: 20px;
	font-family: 'Open Sans';
	font-weight: 700;
	color: #2F3841;
}

.Action{
	font-size: 14px;
	font-family: 'Open Sans';
	font-weight: 600;
	color: #E44C4C;
	cursor: pointer;
	border-bottom: 1px solid #E44C4C;
}

.Cart-Items{
	margin: auto;
	width: 90%;
	height: 30%;
	display: flex;
	justify-content: space-between;
	align-items: center;
}
.image-box{
	width: 15%;
	text-align: center;
}
.about{
	height: 100%;
	width: 24%;
}
.title{
	padding-top: 10px;
	line-height: 10px;
	font-size: 32px;
	font-family: 'Open Sans';
	font-weight: 800;
	color: #202020;
}
.subtitle{
	line-height: 10px;
	font-size: 18px;
	font-family: 'Open Sans';
	font-weight: 600;
	color: #909090;
}

.counter{
	width: 15%;
	display: flex;
	justify-content: space-between;
	align-items: center;
}
.btn{
	width: 40px;
	height: 40px;
	border-radius: 50%;
	background-color: #d9d9d9;
	display: flex;
	justify-content: center;
	align-items: center;
	font-size: 20px;
	font-family: 'Open Sans';
	font-weight: 900;
	color: #202020;
	cursor: pointer;
}
.count{
	font-size: 20px;
	font-family: 'Open Sans';
	font-weight: 600;
	color: #202020;
}

.prices{
	height: 100%;
	text-align: right;
}
.amount{
	padding-top: 20px;
	font-size: 26px;
	font-family: 'Open Sans';
	font-weight: 800;
	color: #202020;
}
.save{
	padding-top: 5px;
	font-size: 14px;
	font-family: 'Open Sans';
	font-weight: 600;
	color: #1687d9;
	cursor: pointer;
}
.remove{
	padding-top: 5px;
	font-size: 14px;
	font-family: 'Open Sans';
	font-weight: 600;
	color: #E44C4C;
	cursor: pointer;
}

.pad{
	margin-top: 5px;
}

hr{
	width: 66%;
	float: right;
	margin-right: 5%;
}
.checkout{
	float: right;
	margin-right: 5%;
	width: 28%;
}
.total{
	width: 100%;
	display: flex;
	justify-content: space-between;
}
.Subtotal{
	font-size: 22px;
	font-family: 'Open Sans';
	font-weight: 700;
	color: #202020;
}
.items{
	font-size: 16px;
	font-family: 'Open Sans';
	font-weight: 500;
	color: #909090;
	line-height: 10px;
}
.total-amount{
	font-size: 36px;
	font-family: 'Open Sans';
	font-weight: 900;
	color: #202020;
}
.button{
	margin-top: 10px;
	width: 100%;
	height: 40px;
	border: none;
	background: linear-gradient(to bottom right, #B8D7FF, #8EB7EB);
	border-radius: 20px;
	cursor: pointer;
	font-size: 16px;
	font-family: 'Open Sans';
	font-weight: 600;
	color: #202020;
}
.modeofpayment{
    width: 200px;
    background-color: #999494;
}

```

## Output

![Screenshot 2023-06-04 114730](https://github.com/Gowri4622/restaurant/assets/75235455/01b8c5de-d4fd-4580-bb76-78900df144fb)
![Screenshot 2023-06-04 114803](https://github.com/Gowri4622/restaurant/assets/75235455/04554999-fd7a-44f6-8ee7-1047ddf82c8e)
![Screenshot 2023-06-04 114828](https://github.com/Gowri4622/restaurant/assets/75235455/35d77d6e-9510-47d1-be20-11dde42371fe)



## Result
Thus we Successfully created Commercial Website using HTML & CSS
