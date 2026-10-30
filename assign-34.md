<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Responsive navbar and hero using Flexbox." >
    <title>Navbar and Hero</title>

    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: Arial, sans-serif;
            color: #1b263b;
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px;
            box-shadow: 0 2px 8px #ddd;
            position: relative;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: #0077b6;
        }

        .links {
            display: flex;
            gap: 20px;
            list-style: none;
        }

        .links a {
            text-decoration: none;
            color: #1b263b;
        }

        .links .cta {
            background: #0077b6;
            color: white;
            padding: 10px;
            border-radius: 5px;
        }

        #toggle,
        .burger {
            display: none;
        }

        .hero {
            display: flex;
            align-items: center;
            justify-content: space-between;
            gap: 30px;
            max-width: 1100px;
            margin: auto;
            padding: 50px 20px;
        }

        .hero-text,
        .hero-img {
            flex: 1;
        }

        .hero-text h1 {
            font-size: 40px;
            margin-bottom: 15px;
        }

        .hero-text p {
            color: #555;
            margin-bottom: 20px;
        }

        .buttons {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn {
            padding: 12px 20px;
            border-radius: 6px;
            text-decoration: none;
        }

        .primary {
            background: #0077b6;
            color: white;
        }

        .secondary {
            border: 2px solid #0077b6;
            color: #0077b6;
        }

        .hero-img img {
            width: 100%;
            border-radius: 15px;
        }

        @media (max-width: 768px) {
            .burger {
                display: block;
                font-size: 28px;
                cursor: pointer;
            }

            .links {
                display: none;
                position: absolute;
                top: 100%;
                left: 0;
                width: 100%;
                background: white;
                padding: 20px;
                flex-direction: column;
            }

            #toggle:checked ~ .links {
                display: flex;
            }

            .hero {
                flex-direction: column-reverse;
                text-align: center;
            }

            .buttons {
                justify-content: center;
            }
        }
    </style>
</head>

<body>

    <nav class="navbar">
        <span class="logo">CloudNine</span>

        <input type="checkbox" id="toggle">
        <label for="toggle" class="burger">☰</label>

        <ul class="links">
            <li><a href="#">Features</a></li>
            <li><a href="#">Pricing</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#" class="cta">Get Started</a></li>
        </ul>
    </nav>

    <header class="hero">

        <div class="hero-text">
            <h1>Build Faster with CloudNine</h1>

            <p>
                Deploy, scale and monitor your apps easily
                without managing servers.
            </p>

            <div class="buttons">
                <a href="#" class="btn primary">Start Free</a>
                <a href="#" class="btn secondary">Watch Demo</a>
            </div>
        </div>

        <div class="hero-img">
            <img src="https://static.vecteezy.com/system/resources/thumbnails/057/377/480/small/a-professional-remote-work-setup-featuring-a-laptop-on-a-wooden-desk-a-cup-of-coffee-and-natural-light-streaming-through-a-window-photo.jpg"
                 alt="Laptop on a desk">
        </div>

    </header>

</body>
</html>
