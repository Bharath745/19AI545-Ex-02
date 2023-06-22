# Ex-07 Create a commercial website using HTML & CSS
## AIM:-
To create a commercial website using HTML & CSS.

## PROCEDURE:-
### STEP 1:
Create basic outline for website using html.

### STEP 2:
Create style part of the website using css.

### STEP 3:
Link the css file with html code using link tag

### STEP 4:
Run the code and check the webpage in an web browser.

## PROGRAM:-
#### Developed By : Bharath V
#### Register Number : 212221230013
### HTML:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Food Website</title>
    <link rel="stylesheet" href="sty.css">
</head>
<body>
    <section id="Home">
        <nav>
            <div class="logo">
                <img src="image/logo.png">
            </div>
            <ul>
                <li><a href="#Home">Home</a></li>
                <li><a href="#About">About</a></li>
                <li><a href="#Catalog">Catalog</a></li>
            </ul>
            <div class="icon">
                <i class="fa-solid fa-magnifying-glass"></i>
                <i class="fa-solid fa-heart"></i>
                <i class="fa-solid fa-cart-shopping"></i>
            </div>
        </nav>
        <div class="main">
            <div class="men_text">
                <h1>Quality Food <br> Delivered!</h1>
            </div>
            <div class="main_image">
                <img src="image/main_img.png">
            </div>
        </div>
        <p>
            Lorem ipsum is simply dummy text of the printing and <br>typesetting industry.Lorem lpsum has been the industry's <br>standard dummy text ever since the 1500s.
        </p>
        <div class="main_btn">
            <a href="#">Get Started</a>
        </div>
    </section>
  
    <!--About-->
    <div class="about" id="About">
        <div class="about_main">
            <div class="image">
                <img src="image/dosa_img.png">
            </div>
            <div class="about_text">
                <h1>Traditional<br> Vegetarian Food</h1>
                <p>
                    Vegetarian food is good for health and thats what we provide<br>
                    here in <span>Foodka</span> as we focus on customers health before<br>
                    money reaches the table.
                </p>
            </div>
        </div>
        <a href="#" class="about_btn">Order Veg Food</a>
    </div>
  
    <!--Review-->
    <div class="review" id="Review">
        <h1>Our Happy Customer</h1>
        <div class="review_box">
            <div class="review_card">
                <div class="review_profile">
                    <img src="image/review_1.png">
                </div>
                <div class="review_text">
                    <h2 class="name">Andrew Banks</h2>
                    <p>
                       "I dont always clop, but when i do,it's
                       because of food.Wow what great food has just
                       not let me leave the store until now for this very minute!"
                    </p>
                </div>
            </div>
            <div class="review_card">
                <div class="review_profile">
                    <img src="image/review_2.png">
                </div>
                <div class="review_text">
                    <h2 class="name">John Morrison</h2>
                    <p>
                        The food here is the one of the human to eat
                        but i do,it's because of food.Wow what 
                        great food has just not let me leave the store  
                        until now for this very minute!"
                    </p>
                </div>
            </div>
                </div>
            </div>
        </div>
    </div>
  
    <!--Footer-->
    <footer>
        <div class="footer_main">
            <div class="footer_tag">
                <h1><span>Food</span>ka</h1>
                <p>The best food for right person</p>
                <h2><span>About us</span></h2>
                <p>we just the food shop which everyone has been waiting.</p>
            </div>
            <div class="footer_tag">
                <h2><span>Quick Link</span> </h2>
                <p>Home</p>
                <p>About</p>
                <p>Menu</p>
                <p>Gallary</p>
                <p>Order</p>
            </div>
            <div class="footer_tag">
                <h2><span>Contact</span></h2>
                <p>+91 7558142745</p>
                <p>+91 9735923857</p>
                <p>bharath@gmail.com</p>
            </div>
            <div class="footer_tag">
                <h2><span>More Links</span></h2>
                <p>Gallery</p>
                <p>Inside our shop</p>
                <p>Pricing</p>
            </div>
            <div class="footer_tag">
                <h2><span>Follow us</span></h2>
                <i class="fa-brands fa-facebook-f"></i>
                <i class="fa-brands fa-twitter"></i>
                <i class="fa-brands fa-instagram"></i>
                <i class="fa-brands fa-linkedin-in"></i>
            </div>
        </div>
    </footer>
</body>
</html>
```
### CSS:
```css
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: sans-serif;
    outline:none;border:none;
    background-color:#f6d7aa ;
}
html{
    scroll-behavior: smooth;
}
section{
    width: 100%;
    height: 80vh;
}
section nav{
    display: flex;
    justify-content: space-around;
    align-items: center;
    position: fixed;
    right: 0;
    left: 0;
    background: #f6d7aa;
    box-shadow: 0 0 10px rgba(0,0,0,0.5);
    z-index: 1000;
}
section nav .logo img{
    width: 100px;
    cursor: pointer;
    margin: 7px 0;
}
section nav ul{
    list-style: none;
}
section nav ul li{
    display: inline-block;
    margin: 0 15px;
}
section nav ul li a{
    text-decoration: none;
    color: #000;
    font-weight: 500;
    font-size: 17px;
    transition: 0.1s;
}
section nav ul li a::after{
    content: '';
    width: 0;
    height: 2px;
    background: #f6d7aa;
    display: block;
    transition: 0.2s linear;
}
section nav ul li a:hover::after{
    width: 100%;
}
section nav ul li a:hover{
    color: #f6d7aa;
}
section nav .icon i{
    font-size: 18px;
    color: #000;
    margin: 0 5px;
    cursor: pointer;
    transition: 0.3s;
}
section nav .icon i:hover{
    color: #f6d7aa;
}
section .main{
    display: flex;
    align-items: center;
    justify-content: space-around;
    position: relative;
    top: 130px;
}

/*About*/
.about{
    width: 100%;
    height: 100vh;
    padding: 70px 0;
}
.about .about_main{
    display: flex;
    align-items: center;
    justify-content: space-around;
}
.about .about_main .image img{
    width: 500px;
    position: relative;
    bottom: 250px;
}
.about .about_main .about_text p span{
    color: #fac031;
}
.about .about_main .about_text h1{
    font-size: 55px;
    position: relative;
    bottom: 300px;
}

/*Review*/
.review{
    width: 100%;
    height: 100vh;
    padding: 70px 0;
}
.review h1{
    font-size: 55px;
    bottom: 500px;
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;
}
.review .review_box{
    bottom: 500px;
    position: relative;
    width: 50%;
    margin: 20px auto;
    display: flex;
}
.review .review_box .review_card{
    width: 650px;
    height: 300px;
    background-color: #eeeeee;
    box-shadow: 0 2px 8px rgba(0,0,0,0.5);
    border-radius: 8px;
    padding: 8px 20px;
    margin: 0 8px;
}
.review .review_box .review_card .review_profile{
    display: flex;
    align-items: baseline;
    background-color: #eeeeee;
    justify-content: flex-start;
    position: relative;
    transition: 0.3s;
}
.review .review_box .review_card .review_profile img{
    width: 80px;
    height: 80px;
    object-fit: cover;
    object-position: center;
    border-radius: 50%;
    border: 5px solid #cccccc;
}


/*Footer*/
footer{
    width: 100%;
    padding: 30px 0 0 20px;
    background:#f6d7aa;
    bottom:600px;
    position: relative;
}
footer .footer_main{
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
}
footer .footer_main .footer_tag{
    text-align: center;
}
footer .footer_main .footer_tag h1 span{
    color: #fac031;
}
footer .footer_main .footer_tag h2 span{
    color: #fac031;
}
footer .footer_main .footer_tag h2{
    color:white;
    margin-bottom: 25px;
    font-size: 30px;
}

```
## OUTPUT:-
![image](https://github.com/Bharath745/19AI545-Ex-02/assets/94508354/8f9ef9c9-037a-4863-96db-b2e4a5f57be8)
![image](https://github.com/Bharath745/19AI545-Ex-02/assets/94508354/458d12ff-ee44-4092-b132-7287ae428ca3)
![image](https://github.com/Bharath745/19AI545-Ex-02/assets/94508354/6b1594a0-174e-4d29-9301-3d918e7e18d1)


## RESULT:-
A commercial website using HTML & CSS has been created and output verified sucessfully.
