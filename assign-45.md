<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Bloom Café – finished, fully responsive landing page.">
    <title>Bloom Café – Responsive Landing Page</title>

    <style>
        :root {
            --cream: #fbf5ec;
            --brown: #4a2c1a;
            --green: #5b8c5a;
            --gold: #d99a2b;
            --radius: 14px;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: Georgia, serif;
            background: var(--cream);
            color: var(--brown);
            line-height: 1.6;
        }

        img {
            max-width: 100%;
            display: block;
        }

        a {
            color: inherit;
            text-decoration: none;
        }

        .wrap {
            width: 92%;
            max-width: 1150px;
            margin: auto;
        }

        .btn {
            display: inline-block;
            background: var(--gold);
            color: white;
            padding: 12px 25px;
            border-radius: 30px;
            font-weight: bold;
        }

        h2 {
            font-size: 32px;
            text-align: center;
            margin-bottom: 30px;
        }

        /* Header */
        .site-header {
            padding: 20px 0;
        }

        .site-header .wrap {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 25px;
            font-weight: bold;
            color: var(--green);
        }

        .site-nav ul {
            display: flex;
            gap: 25px;
            list-style: none;
        }

        .nav-toggle,
        .burger {
            display: none;
        }

        .burger {
            font-size: 30px;
            cursor: pointer;
        }

        .hero .wrap {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: center;
            padding: 60px 0;
        }

        .hero h1 {
            font-size: 50px;
            line-height: 1.2;
            margin-bottom: 15px;
        }

        .hero p {
            margin-bottom: 25px;
            font-size: 18px;
        }

        .hero img {
            width: 100%;
            height: 400px;
            object-fit: cover;
            border-radius: var(--radius);
        }

        .menu {
            padding: 60px 0;
            background: white;
        }

        .menu__grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .dish {
            background: var(--cream);
            border-radius: var(--radius);
            overflow: hidden;
        }

        .dish img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .dish__body {
            padding: 20px;
        }

        .dish__row {
            display: flex;
            justify-content: space-between;
            align-items: baseline;
            gap: 10px;
        }

        .dish__price {
            color: var(--green);
            font-weight: bold;
        }

        .about {
            padding: 60px 0;
        }

        .about .wrap {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: center;
        }

        .about img {
            border-radius: var(--radius);
        }

        .about h2 {
            text-align: left;
        }

        .contact {
            background: var(--green);
            color: white;
            padding: 50px 0;
            text-align: center;
        }

        .contact .btn {
            margin-top: 20px;
        }

        .site-footer {
            padding: 25px 0;
        }

        .site-footer .wrap {
            display: flex;
            justify-content: space-between;
            gap: 15px;
        }

        @media (max-width: 900px) {
            .hero .wrap,
            .about .wrap {
                grid-template-columns: 1fr;
                gap: 30px;
            }

            .hero {
                text-align: center;
            }

            .hero h1 {
                font-size: 40px;
            }

            .hero img {
                height: 300px;
            }

            .menu__grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .about {
                text-align: center;
            }

            .about h2 {
                text-align: center;
            }
        }

        @media (max-width: 600px) {
            .site-header .wrap {
                flex-wrap: wrap;
            }

            .burger {
                display: block;
            }

            .site-nav {
                display: none;
                width: 100%;
            }

           .nav-toggle:checked ~ .site-nav {
                display: block;
            }

            .site-nav ul {
                flex-direction: column;
                gap: 0;
                text-align: center;
            }

            .site-nav a {
                display: block;
                padding: 12px;
                border-top: 1px solid #ddd;
            }

            .hero .wrap {
                padding: 35px 0;
            }

            .hero h1 {
                font-size: 32px;
            }

            .hero img {
                height: 220px;
            }

            h2 {
                font-size: 26px;
            }

            .menu__grid {
                grid-template-columns: 1fr;
            }

            .site-footer .wrap {
                flex-direction: column;
                align-items: center;
                text-align: center;
            }
        }
    </style>
</head>

<body>
   <header class="site-header">
        <div class="wrap">
            <a class="logo" href="#">Bloom Café</a>

            <input type="checkbox" id="nav-toggle" class="nav-toggle">

            <label for="nav-toggle" class="burger">☰</label>

            <nav class="site-nav" aria-label="Main navigation">
                <ul>
                    <li><a href="#menu">Menu</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main>

        <section class="hero">
            <div class="wrap">
                <div>
                    <h1>Fresh coffee. Warm moments.</h1>
                    <p>
                        Small-batch coffee and homemade bakes,
                        served in the heart of Meerut.
                    </p>
                    <a class="btn" href="#menu">See Our Menu</a>
                </div>

                <img
                    src="https://picsum.photos/id/225/800/600"
                    alt="Coffee on a wooden table"
                >
            </div>
        </section>

        <section class="menu" id="menu">
            <div class="wrap">
                <h2>Our Favourites</h2>

                <div class="menu__grid">

                    <article class="dish">
                        <img src="https://picsum.photos/id/1060/500/400"
                             alt="Latte with milk foam">
                        <div class="dish__body">
                            <div class="dish__row">
                                <h3>Signature Latte</h3>
                                <span class="dish__price">₹180</span>
                            </div>
                            <p>Double espresso with steamed milk.</p>
                        </div>
                    </article>

                    <article class="dish">
                        <img src="https://picsum.photos/id/292/500/400"
                             alt="Fresh croissants">
                        <div class="dish__body">
                            <div class="dish__row">
                                <h3>Butter Croissant</h3>
                                <span class="dish__price">₹120</span>
                            </div>
                            <p>Freshly baked, flaky and golden.</p>
                        </div>
                    </article>

                    <article class="dish">
                        <img src="https://picsum.photos/id/312/500/400"
                             alt="Chocolate cake">
                        <div class="dish__body">
                            <div class="dish__row">
                                <h3>Choco Cake</h3>
                                <span class="dish__price">₹210</span>
                            </div>
                            <p>Rich dark chocolate cake.</p>
                        </div>
                    </article>

                </div>
            </div>
        </section>

        <section class="about" id="about">
            <div class="wrap">
                <img src="https://picsum.photos/id/431/700/500"
                     alt="Cosy café interior">

                <div>
                    <h2>Our Story</h2>
                    <p>
                        Bloom Café began as a small stall in 2019.
                        Today, it is a cosy place where students,
                        artists and families enjoy good food and coffee.
                    </p>
                </div>
            </div>
        </section>

       <section class="contact" id="contact">
            <div class="wrap">
                <h2>Visit Us</h2>
                <p>12 Garden Road, Meerut · Open daily 8 AM – 10 PM</p>
                <a class="btn" href="tel:+919000000000">Call to Reserve</a>
            </div>
        </section>

    </main>

    <footer class="site-footer">
        <div class="wrap">
            <span>&copy; 2026 Bloom Café</span>
            <span>Instagram · Facebook</span>
        </div>
    </footer>

</body>
</html>

