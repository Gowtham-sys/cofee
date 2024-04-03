<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>QScript Coffee</title>
    <style>
        /* CSS styles */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f8f8f8;
            color: #333;
        }

        nav {
            background-color: #333;
            padding: 10px 0;
            text-align: center;
        }

        nav ul {
            list-style-type: none;
            margin: 0;
            padding: 0;
        }

        nav ul li {
            display: inline;
            margin-right: 20px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
        }

        .hero {
            background-image: url('C:\Users\mushraf\Downloads\cofeeshop.jpg');
            background-size: cover;
            color: white;
            text-align: center;
            padding: 150px 0;
            position: relative; /* Added */
        }

        .hero img {
            position: absolute; /* Added */
            top: 0;
            left: 0;
            width: 100%;
            height: 39%;
            object-fit: cover;
            z-index: -1;
        }

        .hero h1 {
            font-size: 3.5em;
            margin-bottom: 20px;
            color: black;
        }

        .hero p {
            font-size: 1.2em;
            margin-bottom: 30px;
            color: black;
        }

        .btn {
            display: inline-block;
            padding: 15px 30px;
            background-color: #ff6f61;
            color: white;
            text-decoration: none;
            border-radius: 25px;
            transition: background-color 0.3s ease;
        }

        .btn:hover {
            background-color: #d95042;
        }

        section {
            padding: 50px 20px;
        }

        h2 {
            font-size: 2.5em;
            margin-bottom: 30px;
            text-align: center;
        }

        .menu-item {
            margin-bottom: 40px;
        }

        .menu-item img {
            width: 100%;
            max-width: 300px;
            display: block;
            margin: 0 auto 20px;
            border-radius: 10px;
        }

        .menu-item h3 {
            font-size: 2em;
            margin-bottom: 10px;
            color: #333;
            text-align: center;
        }

        .menu-item p {
            font-size: 1.2em;
            color: #555;
            line-height: 1.5;
        }

        .contact-form {
            max-width: 500px;
            margin: 0 auto;
            background-color: #fff;
            padding: 30px;
            border-radius: 20px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        label {
            display: block;
            margin-bottom: 5px;
            font-size: 1.2em;
        }

        input[type="text"],
        input[type="email"],
        textarea {
            width: calc(100% - 20px);
            padding: 15px;
            border: 1px solid #ccc;
            border-radius: 10px;
            margin-bottom: 15px;
            font-size: 1.1em;
            background-color: #f8f8f8;
            color: #333;
        }

        button[type="submit"] {
            background-color: #ff6f61;
            color: #fff;
            border: none;
            border-radius: 10px;
            padding: 15px 30px;
            cursor: pointer;
            font-size: 1.2em;
            transition: background-color 0.3s ease;
        }

        button[type="submit"]:hover {
            background-color: #d95042;
        }

        .map-container {
            width: 100%;
            height: 400px;
            margin-top: 50px;
        }
    </style>
</head>
<body>
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About Us</a></li>
            <li><a href="#menu">Menu</a></li>
            <li><a href="#contact">Contact Us</a></li>
        </ul>
    </nav>

    <section id="home" class="hero">
        <img src="C:\Users\mushraf\Downloads\cofeeshop.jpg" alt="Cofeeshop">
        <h1>Welcome to QScript Coffee</h1>
        <p>Experience the finest coffee blends and delightful pastries!</p>
        <a href="#contact" class="btn">Contact Us</a>
    </section>

    <section id="about">
        <h2>About Us</h2>
        <p>QScript Coffee is not just a coffee shop; it's an experience. We believe in serving more than just a cup of coffee; we serve memories. Our passionate team curates the finest coffee beans and prepares each cup with love and precision.</p>
        <p>Step into our cozy atmosphere, where the aroma of freshly brewed coffee blends with the scent of freshly baked pastries. Let us be a part of your daily ritual, your moment of indulgence, or your escape from the routine.</p>
    </section>

    <section id="menu">
        <h2>Our Menu</h2>
        <div class="menu-item">
            <img src="C:\Users\mushraf\Downloads\espre.jpg" alt="Espresso">
            <h3>Espresso</h3>
            <p>A concentrated coffee beverage brewed by forcing a small amount of nearly boiling water through finely-ground coffee beans.</p>
        </div>
        <div class="menu-item">
            <img src="cappuccino.jpg" alt="Cappuccino">
            <h3>Cappuccino</h3>
            <p>Espresso mixed with steamed milk foam.</p>
        </div>
        <div class="menu-item">
            <img src="latte.jpg" alt="Latte">
            <h3>Latte</h3>
            <p>Espresso with steamed milk and a small amount of milk foam.</p>
        </div>
        <div class="menu-item">
            <img src="croissant.jpg" alt="Chocolate Croissant">
            <h3>Chocolate Croissant</h3>
            <p>A buttery, flaky pastry filled with rich chocolate.</p>
        </div>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <div class="contact-form">
            <form id="contact-form">
                <div class="form-group">
                    <label for="name">Name:</label>
                    <input type="text" id="name" name="name" required>
                </div>
            
                <div class="form-group">
                    <label for="email">Email:</label>
                    <input type="email" id="email" name="email" required>
                </div>
                <div class="form-group">
                    <label for="message">Message:</label>
                    <textarea id="message" name="message" required></textarea>
                </div>
                <button type="submit">Submit</button>
            </form>
        </div>
    </section>

    <section id="map">
        <h2>Find Us</h2>
        <div class="map-container">
            <!-- Embed your map here -->
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d96793.34637475411!2d-74.0066105!3d40.7143528!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89c2598d76a0f081%3A0xf02af5cf64a4f2b7!2sNew%20York%2C%20NY%2C%20USA!5e0!3m2!1sen!2sin!4v1630527730249!5m2!1sen!2sin" width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
        </div>
    </section>
</body>
</html>
