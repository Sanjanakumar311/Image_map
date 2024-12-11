# Ex04 Places Around Me
# Date:26/10/2024
# AIM
To develop a website to display details about the places around my house.

# DESIGN STEPS
## STEP 1
Create a Django admin interface.

## STEP 2
Download your city map from Google.

## STEP 3
Using <map> tag name the map.

## STEP 4
Create clickable regions in the image using <area> tag.

## STEP 5
Write HTML programs for all the regions identified.

## STEP 6
Execute the programs and publish them.

# CODE
```python
IMAGE MAP CODE:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IMAGE MAP</title>
</head>
<body>
    <img  src="/static/Screenshot 2024-11-28 083941.png" usemap="#mymap">
    <map name="mymap">
        <area shape="rect" coords="649,182,422,83" title="Sports store" href="file:///C:/Users/admin/Image_map/sanjana/mapapp/static/imap1.html">
        <area shape="rect" coords="460,630,219,522" title="Gifts shop" href="file:///C:/Users/admin/Image_map/sanjana/mapapp/static/imap2.html">
        <area shape="rect" coords="1349,787,1108,679" title="Medical store" href="file:///C:/Users/admin/Image_map/sanjana/mapapp/static/imap3.html">
        <area shape="rect" coords="637,381,790,431" title="Gym muscle monster" href="file:///C:/Users/admin/Image_map/sanjana/mapapp/static/imap4.html">
        <area shape="rect" coords="1238,89,1391,139" title="Natural salon center" href="file:///C:/Users/admin/Image_map/sanjana/mapapp/static/imap5.html">
    </map>
        
</body>
</html>

WEBSITE1 CODE:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rebel Sports Store</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
            color: #333;
        }
        header {
            background-color: #007BFF;
            color: white;
            padding: 20px;
            text-align: center;
        }
        .container {
            max-width: 1200px;
            margin: 20px auto;
            padding: 20px;
            background: white;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        .store-image {
            width: 100%;
            height: auto;
            border-radius: 8px;
        }
        .description {
            margin-top: 20px;
        }
        .contact {
            margin-top: 40px;
            background-color: #f1f1f1;
            padding: 20px;
            border-radius: 8px;
        }
        footer {
            text-align: center;
            padding: 20px;
            background-color: #007BFF;
            color: white;
            margin-top: 20px;
        }
        a {
            color: #007BFF;
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>

<header>
    <h1>Welcome to Rebel Sports Store</h1>
    <p>Your one-stop shop for all sports gear and accessories!</p>
</header>

<div class="container">
    <img src="/static/sports shop.jpg" alt="Sports Store" class="store-image">
    <div class="description">
        <h2>About Us</h2>
        <p>
            At Rebel Sports Store, we offer a wide range of high-quality sports equipment, clothing, and accessories for enthusiasts of all levels. 
            Whether you are a professional athlete or just starting your fitness journey, we have something for everyone. 
            Our products include gear for football, basketball, cricket, running, yoga, and more.
        </p>
        <p>
            We are committed to providing top brands, exceptional customer service, and competitive prices to meet your needs.
        </p>
    </div>

    <div class="contact">
        <h3>Contact Us</h3>
        <p><strong>Address:</strong> 123 Nethaji Street,Krishnagiri</p>
        <p><strong>Email:</strong> <a href="mailto:info@rebelsportsstore.com">info@rebelsportsstore.com</a></p>
        <p><strong>Phone:</strong>9874563210</p>
        <p><strong>Business Hours:</strong> Mon - Sat: 9:00 AM - 8:00 PM</p>
    </div>
</div>

<footer>
    <p>&copy; 2024 Rebel Sports Store. All Rights Reserved.</p>
</footer>

</body>
</html>

WEBSITE2 CODE:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gift Shop</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #ff6347;
            color: white;
            padding: 20px;
            text-align: center;
        }

        .container {
            width: 80%;
            margin: 0 auto;
        }

        .shop-image {
            width: 100%;
            height: auto;
        }

        .shop-description {
            background-color: white;
            padding: 20px;
            margin-top: 20px;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        .contact-details {
            background-color: #fff;
            padding: 20px;
            margin-top: 20px;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        footer {
            background-color: #ff6347;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }

        .contact-details ul {
            list-style-type: none;
            padding: 0;
        }

        .contact-details li {
            padding: 5px 0;
        }
    </style>
</head>
<body>

    <header>
        <h1>Welcome to Our Rekh's Gift Shop</h1>
        <p>Your one-stop destination for unique and thoughtful gifts!</p>
    </header>

    <div class="container">
        <!-- Shop Image -->
        <img src="/static/gi.avif" alt="Rekh's Gift Shop" class="shop-image">

        <!-- Shop Description -->
        <div class="shop-description">
            <h2>About Our Gift Shop</h2>
            <p>At our Gift Shop, we offer a wide range of hand-picked gifts for every occasion. From birthdays to anniversaries, our collection is designed to bring a smile to your loved ones. Explore our curated selection of personalized gifts, stylish home decor, and unique accessories that make perfect presents.</p>
            <p>We believe in quality and craftsmanship, ensuring every gift is as special as the recipient. Our team is passionate about helping you find the perfect gift, whether you're shopping for a friend, family member, or someone special.</p>
        </div>

        <!-- Contact Details -->
        <div class="contact-details">
            <h2>Contact Us</h2>
            <p>We would love to hear from you! Whether you have a question, need assistance with your order, or want to share feedback, feel free to get in touch:</p>
            <ul>
                <li><strong>Email:</strong> contact@rekh'sgiftshop.com</li>
                <li><strong>Phone:</strong> 987654321</li>
                <li><strong>Address:</strong> 123 Gift Avenue, Krishnagiri</li>
            </ul>
        </div>
    </div>

    <footer>
        <p>&copy; Rekh's Gift Shop. All Rights Reserved.</p>
    </footer>

</body>
</html>

WEBSITE3 CODE:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ABC Medical Shop</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #4CAF50;
            color: white;
            text-align: center;
            padding: 20px 0;
        }
        .container {
            padding: 20px;
            max-width: 800px;
            margin: auto;
        }
        .shop-image {
            display: block;
            margin: 0 auto 20px;
            max-width: 100%;
            height: auto;
            border-radius: 10px;
        }
        .description {
            margin-bottom: 20px;
            text-align: justify;
        }
        .contact-details {
            background-color: #f9f9f9;
            padding: 15px;
            border-radius: 5px;
        }
        footer {
            text-align: center;
            padding: 10px 0;
            background-color: #4CAF50;
            color: white;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to SSS Medical Shop</h1>
    </header>
    <div class="container">
        <img src="/static/m.webp" alt="Medical Shop" class="shop-image">
        <div class="description">
            <h2>About Us</h2>
            <p>
                ABC Medical Shop is your trusted pharmacy and healthcare destination. We offer a wide range of prescription medicines, over-the-counter drugs, and medical equipment. Our mission is to ensure your health and well-being by providing quality products and exceptional customer service. We are committed to meeting your needs with personalized care and attention.
            </p>
            <p>
                Our experienced staff is always ready to assist you with expert advice and recommendations. Visit us today to experience reliable healthcare solutions for you and your family.
            </p>
        </div>
        <div class="contact-details">
            <h2>Contact Us</h2>
            <p><strong>Address:</strong> 123 Health Avenue, Krishnagiri</p>
            <p><strong>Phone:</strong> 987654321</p>
            <p><strong>Email:</strong> contact@sssmedicalshop.com</p>
            <p><strong>Hours:</strong> Monday to Saturday: 9:00 AM - 8:00 PM<br>Sunday: 10:00 AM - 5:00 PM</p>
        </div>
    </div>
    <footer>
        <p>&copy; 2024 SSS Medical Shop. All Rights Reserved.</p>
    </footer>
</body>
</html>

WEBSITE4 CODE:
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Muscle Gym Center</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f4f4f4;
      color: #333;
    }

    header {
      background-color: #222;
      color: white;
      padding: 20px 10px;
      text-align: center;
    }

    header h1 {
      margin: 0;
    }

    .container {
      max-width: 1200px;
      margin: 20px auto;
      padding: 20px;
      background: white;
      border-radius: 8px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    }

    .image-section img {
      width: 100%;
      max-height: 400px;
      object-fit: cover;
      border-radius: 8px;
    }

    .description {
      margin: 20px 0;
    }

    .contact-details {
      background-color: #f8f9fa;
      padding: 15px;
      border-radius: 8px;
    }

    .contact-details h3 {
      margin-top: 0;
    }

    footer {
      text-align: center;
      padding: 10px;
      background-color: #222;
      color: white;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Welcome to Gym Muscle Monster</h1>
    <p>Your ultimate destination for fitness and strength!</p>
  </header>

  <div class="container">
    <div class="image-section">
      <img src="/static/g.jpg" alt="Gym Image">
    </div>

    <div class="description">
      <h2>About Us</h2>
      <p>
        At Muscle Gym Monster, we believe in empowering individuals to achieve their fitness goals. 
        Our state-of-the-art facilities include cutting-edge equipment, a spacious workout area, 
        and certified trainers dedicated to helping you build strength, endurance, and confidence.
      </p>
      <p>
        Whether you're a beginner or an experienced athlete, we have personalized programs tailored 
        to your needs. Join our vibrant community and take your fitness journey to the next level!
      </p>
    </div>

    <div class="contact-details">
      <h3>Contact Us</h3>
      <p><strong>Address:</strong> 123 Fitness Avenue, Workout City, WC 45678</p>
      <p><strong>Phone:</strong>  9876543210</p>
      <p><strong>Email:</strong> contact@gymmusclemonster.com</p>
      <p><strong>Opening Hours:</strong> Mon-Fri: 6:00 AM - 10:00 PM | Sat-Sun: 8:00 AM - 8:00 PM</p>
    </div>
  </div>

  <footer>
    &copy; 2024 Muscle Gym Center. All rights reserved.
  </footer>
</body>
</html>

WEBSITE5 CODE:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Natural Bliss Salon</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9;
            color: #333;
        }
        header {
            background-color: #6f9e72;
            color: white;
            text-align: center;
            padding: 1rem 0;
        }
        header h1 {
            margin: 0;
            font-size: 2.5rem;
        }
        .main-content {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 2rem;
        }
        .main-content img {
            max-width: 100%;
            height: auto;
            border-radius: 10px;
            margin-bottom: 2rem;
        }
        .description {
            max-width: 800px;
            text-align: center;
            margin-bottom: 2rem;
        }
        .contact-details {
            background-color: #6f9e72;
            color: white;
            padding: 1.5rem;
            text-align: center;
            border-radius: 10px;
            width: 80%;
        }
        .contact-details h2 {
            margin: 0 0 1rem;
        }
        footer {
            text-align: center;
            padding: 1rem;
            background-color: #333;
            color: white;
            margin-top: 2rem;
        }
    </style>
</head>
<body>

<header>
    <h1>Natural Salon center</h1>
    <p>Your sanctuary for organic beauty and wellness</p>
</header>

<div class="main-content">
    <img src="/static/a.jpg" alt="Natural salon center">
    <div class="description">
        <p>Welcome to Natural Bliss Salon, where beauty meets nature. Our mission is to provide premium salon services using organic and eco-friendly products. From rejuvenating hair treatments to soothing skincare rituals, we ensure a holistic and sustainable approach to beauty. Let us help you unwind in a serene environment designed to relax your mind, body, and soul.</p>
    </div>
    <div class="contact-details">
        <h2>Contact Us</h2>
        <p><strong>Phone:</strong> 9123456780</p>
        <p><strong>Email:</strong> contact@naturalsaloncenter.com</p>
        <p><strong>Address:</strong> 123 Green Street, Wellness City, NY 56789</p>
        <p>Follow us on social media for the latest updates and promotions!</p>
    </div>
</div>

<footer>
    <p>&copy; 2024 Natural Salon <center></center>. All rights reserved.</p>
</footer>

</body>
</html>

```
# OUTPUT
IMAGE MAP:
![Screenshot 2024-12-11 152145](https://github.com/user-attachments/assets/398b0f25-2050-48c1-8446-de103784ca6c)
WEBSITE 1:
![Screenshot 2024-12-10 210028](https://github.com/user-attachments/assets/eeb71f76-dccd-43af-801c-f31438273bbf)
![Screenshot 2024-12-10 210045](https://github.com/user-attachments/assets/aed61e6b-fca4-4859-8cdb-7689672bcf98)
WEBSITE 2:
![Screenshot 2024-12-10 210150](https://github.com/user-attachments/assets/eb830398-1f9f-4d30-96e4-f18eba05f6c0)
![Screenshot 2024-12-10 210220](https://github.com/user-attachments/assets/1463a110-3fc9-4953-a6f7-a3b46f668949)
WEBSITE 3:
![Screenshot 2024-12-10 210312](https://github.com/user-attachments/assets/ceec3a27-56ac-41ea-a9dd-d91ec443097b)
![Screenshot 2024-12-10 210327](https://github.com/user-attachments/assets/38442e05-6c41-41a6-9e15-bd9971ac71fb)
WEBSITE 4:
![Screenshot 2024-12-10 210409](https://github.com/user-attachments/assets/92f88db1-d0f9-4f2f-a953-ab04f3676232)
![Screenshot 2024-12-10 210426](https://github.com/user-attachments/assets/00a31d5e-8012-4315-b75f-89ed7fd77b2e)
WEBSITE 5:
![Screenshot 2024-12-10 210505](https://github.com/user-attachments/assets/c56a7874-6742-419c-98bf-1b64927365da)
![Screenshot 2024-12-10 210520](https://github.com/user-attachments/assets/fe0eb95e-3410-4dee-8da1-966f45d17cc4)


# RESULT
The program for implementing image maps using HTML is executed successfully.
