<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TaskFlow – Grid and Flexbox</title>

    <style>
        * {
            box-sizing: border-box;
            margin: 0;
        }

        :root {
            --blue: #3a5bff;
            --dark: #0f1535;
        }

        body {
            font-family: Arial, sans-serif;
            color: var(--dark);
            line-height: 1.6;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        .wrap {
            width: 92%;
            max-width: 1100px;
            margin: auto;
        }

        .nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: var(--blue);
        }

        .nav ul {
            display: flex;
            align-items: center;
            gap: 20px;
            list-style: none;
        }

        .btn {
            display: inline-block;
            padding: 10px 20px;
            background: var(--blue);
            color: white;
            border-radius: 8px;
            font-weight: bold;
        }

        .btn--ghost {
            background: white;
            color: var(--blue);
            border: 2px solid var(--blue);
        }

        .hero {
            display: grid;
            grid-template-columns: 1fr 1fr;
            align-items: center;
            gap: 40px;
            padding: 60px 0;
        }

        .hero h1 {
            font-size: clamp(30px, 5vw, 50px);
            line-height: 1.2;
            margin-bottom: 15px;
        }

        .hero p {
            margin-bottom: 20px;
            color: #4b5280;
        }

        .btns {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
        }

        .hero img {
            width: 100%;
            height: auto;
            border-radius: 15px;
        }

        .features {
            background: #f2f4ff;
            padding: 50px 0;
        }

        .features h2,
        .pricing h2 {
            text-align: center;
            margin-bottom: 30px;
        }

        .features__grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 20px;
        }

        .feature {
            display: flex;
            align-items: flex-start;
            gap: 15px;
            background: white;
            padding: 20px;
            border-radius: 12px;
        }

        .feature span {
            font-size: 30px;
        }

        .pricing {
            padding-top: 50px;
            padding-bottom: 50px;
        }

        .pricing__grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        .plan {
            display: flex;
            flex-direction: column;
            gap: 12px;
            padding: 25px;
            border: 1px solid #d8dcf5;
            border-radius: 12px;
            text-align: center;
        }

        .price {
            font-size: 32px;
            font-weight: bold;
        }

        .plan .btn {
            margin-top: auto;
        }

        .plan--pop {
            border: 2px solid var(--blue);
            box-shadow: 0 10px 25px rgba(58, 91, 255, 0.2);
        }

        footer {
            background: var(--dark);
            color: #cdd2f5;
            padding: 20px 0;
        }

        footer .wrap {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 10px;
        }

        @media (max-width: 820px) {
            .hero {
                grid-template-columns: 1fr;
                text-align: center;
            }

            .btns {
                justify-content: center;
            }

            .pricing__grid {
                grid-template-columns: 1fr;
            }

            .nav ul {
                display: none;
            }
        }
    </style>
</head>

<body>

    <nav>
        <div class="nav">
            <span class="logo">TaskFlow</span>

            <ul>
                <li><a href="#features">Features</a></li>
                <li><a href="#pricing">Pricing</a></li>
                <li><a class="btn" href="#">Sign up</a></li>
            </ul>
        </div>
    </nav>

    <header class="hero">
        <div>
            <h1>Manage every task in one calm place.</h1>
            <p>Plan projects, assign work and meet deadlines without chaos.</p>

            <div class="btns">
                <a class="btn" href="#">Get started</a>
                <a class="btn btn--ghost" href="#">Book a demo</a>
            </div>
        </div>

        <img src="https://picsum.photos/id/0/700/520"alt="Person working on a laptop">
    </header>

   <section class="features" id="features">
        <div class="wrap">
            <h2>Why teams love TaskFlow</h2>

            <div class="features__grid">
                <div class="feature">
                    <div>
                        <h3>Simple boards</h3>
                        <p>Move tasks between stages.</p>
                    </div>
                </div>

                <div class="feature">
                    <div>
                        <h3>Smart reminders</h3>
                        <p>Never miss a deadline.</p>
                    </div>
                </div>

                <div class="feature">
                    <div>
                        <h3>Team sharing</h3>
                        <p>Assign tasks and work together.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section class="pricing wrap" id="pricing">
        <h2>Pricing</h2>

        <div class="pricing__grid">
            <div class="plan">
                <h3>Free</h3>
                <p class="price">₹0</p>
                <p>1 project · 3 members</p>
                <a class="btn btn--ghost" href="#">Choose</a>
            </div>

            <div class="plan plan--pop">
                <h3>Pro</h3>
                <p class="price">₹499</p>
                <p>Unlimited projects · 20 members · Priority support</p>
                <a class="btn" href="#">Choose</a>
            </div>

            <div class="plan">
                <h3>Team</h3>
                <p class="price">₹1,499</p>
                <p>Unlimited features</p>
                <a class="btn btn--ghost" href="#">Choose</a>
            </div>
        </div>
    </section>

    <footer>
        <div class="wrap">
            <span>&copy; 2026 TaskFlow</span>
            <span>Privacy · Terms</span>
        </div>
    </footer>

</body>
</html>
