<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Finished Flexbox landing-page: nav, hero, features, testimonials and footer.">
    <title>FitLife Landing Page</title>

    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: Arial, sans-serif;
            color: #222;
            line-height: 1.6;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        .container {
            max-width: 1100px;
            margin: auto;
            padding: 0 20px;
        }

        nav .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding-top: 15px;
            padding-bottom: 15px;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: #2d6a4f;
        }

        nav ul {
            display: flex;
            gap: 25px;
            list-style: none;
        }

        .hero {
            background: #d8f3dc;
        }

        .hero .container {
            display: flex;
            align-items: center;
            gap: 30px;
            padding-top: 50px;
            padding-bottom: 50px;
        }

        .hero-text,
        .hero-img {
            flex: 1;
        }

        .hero h1 {
            font-size: 40px;
            color: #1b4332;
            margin-bottom: 15px;
        }

        .hero p {
            margin-bottom: 20px;
        }

        .btn {
            display: inline-block;
            background: #ff9f1c;
            padding: 12px 25px;
            border-radius: 25px;
            font-weight: bold;
        }

        .hero-img img {
            width: 100%;
            border-radius: 15px;
        }

        .features {
            padding: 50px 0;
            text-align: center;
        }

        .features h2 {
            color: #1b4332;
            margin-bottom: 30px;
        }

        .features-list {
            display: flex;
            gap: 20px;
            flex-wrap: wrap;
        }

        .feature {
            flex: 1 1 250px;
            padding: 25px;
            border: 1px solid #ddd;
            border-radius: 12px;
        }

        .feature span {
            font-size: 35px;
        }

        .feature h3 {
            margin: 10px 0;
        }

        .testimonial {
            background: #1b4332;
            color: white;
            padding: 40px 0;
        }

        .testimonial .container {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
        }

        .quote {
            flex: 1 1 300px;
        }

        .quote cite {
            display: block;
            margin-top: 10px;
            color: #ff9f1c;
        }

        footer .container {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 10px;
            padding-top: 20px;
            padding-bottom: 20px;
            color: #666;
        }

        @media (max-width: 768px) {
            nav ul {
                display: none;
            }

            .hero .container {
                flex-direction: column;
                text-align: center;
            }
        }
    </style>
</head>

<body>

    <nav>
        <div class="container">
            <span class="logo">FitLife</span>

            <ul>
                <li><a href="#features">Features</a></li>
                <li><a href="#stories">Stories</a></li>
                <li><a href="#">Join</a></li>
            </ul>
        </div>
    </nav>

    <header class="hero">
        <div class="container">

            <div class="hero-text">
                <h1>Train Smarter. Live Stronger.</h1>

                <p>
                    Personalised workouts and meal plans
                    that fit your schedule.
                </p>

                <a href="#" class="btn">Start Free Trial</a>
            </div>

            <div class="hero-img">
                <img src="https://png.pngtree.com/png-clipart/20250518/original/pngtree-cartoon-cute-panda-sitting-happily-with-playful-expression-png-image_21022434.png"
                     alt="A dog resting on a rug">
            </div>

        </div>
    </header>

    <section class="features" id="features">
        <div class="container">

            <h2>Everything You Need</h2>

            <div class="features-list">

                <div class="feature">
                    <span>🏋️</span>
                    <h3>Custom Workouts</h3>
                    <p>Workout plans for your level and equipment.</p>
                </div>

                <div class="feature">
                    <span>🥗</span>
                    <h3>Meal Plans</h3>
                    <p>Simple and balanced recipes.</p>
                </div>

                <div class="feature">
                    <span>📈</span>
                    <h3>Progress Tracking</h3>
                    <p>Track your progress and stay motivated.</p>
                </div>

            </div>
        </div>
    </section>

    <section class="testimonial" id="stories">
        <div class="container">

            <blockquote class="quote">
                “The workouts are easy to follow and enjoyable.”
                <cite>— Riya, Delhi</cite>
            </blockquote>

            <blockquote class="quote">
                “Short and effective workouts.”
                <cite>— Kabir, Meerut</cite>
            </blockquote>

        </div>
    </section>

    <footer>
        <div class="container">
            <span>&copy; 2026 FitLife</span>
        </div>
    </footer>

</body>
</html>
