# Ex02 Commercial Website
## Date:

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
## index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Coffee Shop Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Header -->

    <header>
        <div class="logo">Coffee Corner</div>

        <nav>
            <ul>a
                <li><a href="#home">Home</a></li>
                <li><a href="#products">Coffee Menu</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->

    <section class="hero" id="home">
        <div class="hero-text">
            <h1>Fresh Coffee Everyday</h1>
            <p>Enjoy the best coffee experience with us</p>
            <button>Order Now</button>
        </div>
    </section>

    <!-- Products Section -->

    <section class="products" id="products">

        <h2>Our Coffee Menu</h2>

        <div class="product-container">

            <!-- Product 1 -->

            <div class="product-card">
                <img src="images/product1.jpg" alt="Espresso">
                <h3>Espresso</h3>
                <p>Strong and rich espresso coffee.</p>
                <button>Buy Now</button>
            </div>

            <!-- Product 2 -->

            <div class="product-card">
                <img src="images/product2.jpg" alt="Cappuccino">
                <h3>Cappuccino</h3>
                <p>Creamy cappuccino with milk foam.</p>
                <button>Buy Now</button>
            </div>

            <!-- Product 3 -->

            <div class="product-card">
                <img src="images/product3.jpg" alt="Latte">
                <h3>Latte</h3>
                <p>Smooth latte with fresh milk.</p>
                <button>Buy Now</button>
            </div>

            <!-- Product 4 -->

            <div class="product-card">
                <img src="images/product4.jpg" alt="Mocha">
                <h3>Mocha</h3>
                <p>Chocolate flavored coffee delight.</p>
                <button>Buy Now</button>
            </div>

            <!-- Product 5 -->

            <div class="product-card">
                <img src="images/product5.jpg" alt="Cold Coffee">
                <h3>Cold Coffee</h3>
                <p>Refreshing chilled coffee drink.</p>
                <button>Buy Now</button>
            </div>

        </div>

    </section>

    <!-- About Section -->

    <section class="about" id="about">

        <h2>About Us</h2>

        <p>
            Coffee Corner is a modern coffee shop website created using HTML and CSS Flexbox.
            We provide premium quality coffee with fresh ingredients and excellent service.
        </p>

    </section>

    <!-- Contact Section -->

    <section class="contact" id="contact">

        <h2>Contact Us</h2>

        <div class="contact-box">
            <p><strong>Email:</strong> coffeecorner@gmail.com</p>
            <p><strong>Phone:</strong> +91 9876543210</p>
            <p><strong>Location:</strong> Chennai, Tamil Nadu</p>
        </div>

    </section>

    <!-- Footer -->

    <footer>

        <div class="social-links">
            <a href="#">Facebook</a>
            <a href="#">Instagram</a>
            <a href="#">Twitter</a>
        </div>

        <p>© 2026 Coffee Corner. All Rights Reserved.</p>

    </footer>

</body>
</html>
```
## style.css
```
/* Global Styles */

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body{
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    color: #333;
}

/* Header */

header{
    background-color: #1e293b;
    color: white;
    padding: 20px 50px;

    display: flex;
    justify-content: space-between;
    align-items: center;

    position: sticky;
    top: 0;
}

.logo{
    font-size: 28px;
    font-weight: bold;
}

nav ul{
    display: flex;
    list-style: none;
    gap: 20px;
}

nav ul li a{
    text-decoration: none;
    color: white;
    transition: 0.3s;
}

nav ul li a:hover{
    color: #38bdf8;
}

/* Hero Section */

.hero{
    height: 90vh;
    background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)),
    url('images/banner.jpg');

    background-size: cover;
    background-position: center;

    display: flex;
    justify-content: center;
    align-items: center;

    text-align: center;
    color: white;
}

.hero-text h1{
    font-size: 60px;
    margin-bottom: 20px;
}

.hero-text p{
    font-size: 24px;
    margin-bottom: 20px;
}

.hero button{
    padding: 12px 25px;
    border: none;
    background-color: #38bdf8;
    color: white;
    font-size: 18px;
    border-radius: 5px;
    cursor: pointer;
    transition: 0.3s;
}

.hero button:hover{
    background-color: #0ea5e9;
    transform: scale(1.05);
}

/* Products Section */

.products{
    padding: 60px 40px;
    text-align: center;
}

.products h2{
    margin-bottom: 40px;
    font-size: 40px;
}

.product-container{
    display: flex;
    justify-content: center;
    gap: 30px;
    flex-wrap: wrap;
}

.product-card{
    background-color: white;
    width: 300px;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0px 4px 10px rgba(0,0,0,0.2);
    transition: 0.3s;
}

.product-card:hover{
    transform: translateY(-10px);
}

.product-card img{
    width: 100%;
    height: 220px;
    object-fit: cover;
}

.product-card h3{
    margin-top: 15px;
}

.product-card p{
    padding: 10px;
}

.product-card button{
    margin-bottom: 20px;
    padding: 10px 20px;
    border: none;
    background-color: #1e293b;
    color: white;
    border-radius: 5px;
    cursor: pointer;
}

.product-card button:hover{
    background-color: #334155;
}

/* About Section */

.about{
    padding: 60px 40px;
    background-color: #e2e8f0;
    text-align: center;
}

.about h2{
    margin-bottom: 20px;
    font-size: 40px;
}

/* Contact Section */

.contact{
    padding: 60px 40px;
    text-align: center;
}

.contact h2{
    margin-bottom: 20px;
    font-size: 40px;
}

.contact-box{
    background-color: white;
    width: 400px;
    margin: auto;
    padding: 30px;
    border-radius: 10px;
    box-shadow: 0px 4px 10px rgba(0,0,0,0.2);
}

/* Account Section */

.account{
    padding: 60px 40px;
    background-color: #e2e8f0;
    text-align: center;
}

.account h2{
    margin-bottom: 20px;
    font-size: 40px;
}

.account form{
    display: flex;
    flex-direction: column;
    width: 300px;
    margin: auto;
    gap: 15px;
}

.account input{
    padding: 12px;
    border-radius: 5px;
    border: 1px solid gray;
}

.account button{
    padding: 12px;
    border: none;
    background-color: #1e293b;
    color: white;
    border-radius: 5px;
    cursor: pointer;
}

.account button:hover{
    background-color: #334155;
}

/* Footer */

footer{
    background-color: #1e293b;
    color: white;
    text-align: center;
    padding: 20px;
}

.social-links{
    margin-bottom: 10px;
}

.social-links a{
    color: white;
    text-decoration: none;
    margin: 0 10px;
    transition: 0.3s;
}

.social-links a:hover{
    color: #38bdf8;
}

/* Responsive Design */

@media(max-width: 768px){

    header{
        flex-direction: column;
        gap: 15px;
    }

    nav ul{
        flex-direction: column;
        text-align: center;
    }

    .hero-text h1{
        font-size: 40px;
    }

    .contact-box{
        width: 90%;
    }
}
```


## OUTPUT
<img width="1876" height="901" alt="image" src="https://github.com/user-attachments/assets/99ef4263-12b2-4d37-bea0-06d3cc445de1" />
<img width="1875" height="649" alt="Screenshot 2026-05-25 084313" src="https://github.com/user-attachments/assets/c2919739-89d7-48cb-8c2c-3a7fa1e34dc8" />
<img width="1378" height="510" alt="Screenshot 2026-05-25 084320" src="https://github.com/user-attachments/assets/90de6528-ea57-4798-b83e-757076147b40" />
<img width="1873" height="776" alt="image" src="https://github.com/user-attachments/assets/d13b31c4-9cdb-44a9-86dc-01beda9937c8" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
