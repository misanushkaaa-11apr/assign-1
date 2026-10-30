<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hero Section</title>

    <style>
        * {
            box-sizing: border-box;
            margin: 0;
        }

        body {
            font-family: Arial, sans-serif;
        }

        /* Hero section */
        .hero {
            position: relative;
            height: 100vh;
            min-height: 500px;
            overflow: hidden;
            color: white;
        }

        /* Background image */
        .bg {
            position: absolute;
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        /* Dark overlay */
        .hero::before {
            content: "";
            position: absolute;
            inset: 0;
            background: rgba(0, 0, 0, 0.5);
            z-index: 1;
        }

        /* Navigation bar */
        .nav {
            position: absolute;
            top: 0;
            width: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px;
            z-index: 2;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
        }

        .nav a {
            color: white;
            text-decoration: none;
            margin-left: 15px;
        }

        /* Center content */
        .content {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            text-align: center;
            width: 90%;
            z-index: 2;
        }

        .content h1 {
            font-size: 40px;
            margin-bottom: 15px;
        }

        .content p {
            margin-bottom: 25px;
        }

        /* Button */
        .btn {
            display: inline-block;
            background: coral;
            color: white;
            padding: 12px 25px;
            border-radius: 25px;
            text-decoration: none;
        }

        /* Rating badge */
        .badge {
            position: absolute;
            right: 20px;
            bottom: 20px;
            z-index: 2;
            background: white;
            color: black;
            padding: 15px;
            border-radius: 10px;
        }

        /* Back to top button */
        .top {
            position: fixed;
            right: 15px;
            top: 50%;
            background: white;
            color: black;
            padding: 10px;
            border-radius: 50%;
            text-decoration: none;
            z-index: 5;
        }

        /* Next section */
        .next {
            padding: 60px 20px;
            text-align: center;
        }
    </style>
</head>

<body>

    <header class="hero">

        <img class="bg"
             src="https://picsum.photos/id/1036/1600/900"
             alt="Snowy mountains">

        <nav class="nav">
            <span class="logo">TravelNest</span>

            <div>
                <a href="#">Destinations</a>
                <a href="#">Deals</a>
                <a href="#">Contact</a>
            </div>
        </nav>

        <div class="content">
            <h1>Find Your Next Adventure</h1>
            <p>Explore the world's most beautiful places.</p>
            <a href="#next" class="btn">Start Exploring</a>
        </div>

        <div class="badge">
            <strong>4.9★</strong>
            Happy Travellers
        </div>

    </header>

    <a href="#" class="top">↑</a>

    <section class="next" id="next">
        <h2>Popular Destinations</h2>
        <p>Explore our popular travel destinations.</p>
    </section>

</body>
</html>
