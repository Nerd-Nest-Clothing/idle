<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nerd Nest | Geeky Apparel & Accessories</title>
    <style>
        /* Brand Colors */
        :root {
            --primary: #2ecc71;  /* Geek green */
            --secondary: #e67e22; /* Pumpkin orange */
            --dark: #2c3e50;     /* Dark blue */
            --light: #ecf0f1;    /* Light gray */
        }

        /* Global Styles */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9;
            color: #333;
        }

        /* Header */
        header {
            background-color: var(--dark);
            color: white;
            padding: 1rem 0;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }

        .logo {
            font-size: 2rem;
            font-weight: bold;
            color: var(--primary);
        }

        .logo span {
            color: var(--secondary);
        }

        /* Navigation */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            margin-left: 1.5rem;
            font-weight: 500;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, var(--dark) 0%, var(--primary) 100%);
            color: white;
            padding: 4rem 0;
            text-align: center;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 2rem;
        }

        .btn {
            display: inline-block;
            background-color: var(--secondary);
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 4px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s ease;
        }

        .btn:hover {
            background-color: #d35400;
            transform: translateY(-2px);
        }

        /* Products Section */
        .products {
            padding: 4rem 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            color: var(--dark);
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 2rem;
        }

        .product-card {
            background: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }

        .product-card:hover {
            transform: translateY(-5px);
        }

        .product-img {
            height: 250px;
            background-color: #eee;
            background-size: cover;
            background-position: center;
        }

        .product-info {
            padding: 1.5rem;
        }

        .product-title {
            font-size: 1.2rem;
            margin: 0 0 0.5rem;
        }

        .product-price {
            color: var(--secondary);
            font-weight: bold;
            font-size: 1.1rem;
        }

        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 3rem 0 1rem;
            text-align: center;
        }

        .social-links {
            margin: 1rem 0;
        }

        .social-links a {
            color: white;
            margin: 0 10px;
            font-size: 1.5rem;
        }

        .copyright {
            margin-top: 2rem;
            color: rgba(255,255,255,0.7);
            font-size: 0.9rem;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <nav>
                <div class="logo">Nerd<span>Nest</span></div>
                <div class="nav-links">
                    <a href="#products">Shop</a>
                    <a href="#about">About</a>
                    <a href="#contact">Contact</a>
                </div>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h1>Geek Out in Style</h1>
            <p>High-quality apparel and accessories for gamers, anime lovers, and pop culture fanatics. Wear your fandom with pride!</p>
            <a href="#products" class="btn">Shop Now</a>
        </div>
    </section>

    <!-- Products Section -->
    <section class="products" id="products">
        <div class="container">
            <h2 class="section-title">Featured Products</h2>
            <div class="product-grid">
                <!-- Product 1 -->
                <div class="product-card">
                    <div class="product-img" style="background-image: url('https://via.placeholder.com/500x500');"></div>
                    <div class="product-info">
                        <h3 class="product-title">Pixel Heart Tee</h3>
                        <p class="product-price">$24.99</p>
                    </div>
                </div>
                
                <!-- Product 2 -->
                <div class="product-card">
                    <div class="product-img" style="background-image: url('https://via.placeholder.com/500x500');"></div>
                    <div class="product-info">
                        <h3 class="product-title">Anime All-Star Hoodie</h3>
                        <p class="product-price">$39.99</p>
                    </div>
                </div>
                
                <!-- Product 3 -->
                <div class="product-card">
                    <div class="product-img" style="background-image: url('https://via.placeholder.com/500x500');"></div>
                    <div class="product-info">
                        <h3 class="product-title">Game Over Dad Hat</h3>
                        <p class="product-price">$19.99</p>
                    </div>
                </div>
                
                <!-- Product 4 -->
                <div class="product-card">
                    <div class="product-img" style="background-image: url('https://via.placeholder.com/500x500');"></div>
                    <div class="product-info">
                        <h3 class="product-title">Coding Socks</h3>
                        <p class="product-price">$14.99</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="logo">Nerd<span>Nest</span></div>
            <div class="social-links">
                <a href="#">📱</a>
                <a href="#">📘</a>
                <a href="#">📸</a>
                <a href="#">🐦</a>
            </div>
            <p class="copyright">© 2023 Nerd Nest. All your geek needs in one place.</p>
        </div>
    </footer>
</body>
</html>
