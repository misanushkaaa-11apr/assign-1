<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Three card variants using border-radius and backgrounds.">
    <title>Three Card Variants</title>

    <style>
        * {
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background: #eceff4;
            padding: 20px;
        }

        h1 {
            text-align: center;
        }

        .cards {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }

        .card {
            width: 260px;
            padding: 20px;
        }

        /* Card 1 */
        .soft {
            background: white;
            border-radius: 20px;
            box-shadow: 0 5px 10px #ccc;
        }

        .soft a {
            background: blue;
            color: white;
            border-radius: 20px;
            padding: 8px 15px;
            text-decoration: none;
        }

        /* Card 2 */
        .gradient {
            background: linear-gradient(pink, lightcoral);
            border-radius: 0 40px 0 40px;
        }

        .gradient a {
            background: darkred;
            color: white;
            padding: 8px 15px;
            text-decoration: none;
            border-radius: 5px;
        }

        /* Card 3 */
        .outline {
            background: #1b1b2f;
            color: white;
            border: 2px solid cyan;
            border-radius: 6px;
        }

        .outline a {
            color: cyan;
            border: 2px solid cyan;
            padding: 8px 15px;
            text-decoration: none;
        }

        .outline a:hover {
            background: cyan;
            color: black;
        }
    </style>
</head>

<body>

    <h1>Card Variants</h1>

    <div class="cards">

        <div class="card soft">
            <h2>Soft</h2>
            <p>White background, rounded corners and a shadow.</p>
            <a href="#">Read More</a>
        </div>

        <div class="card gradient">
            <h2>Gradient</h2>
            <p>Colorful background with two rounded corners.</p>
            <a href="#">Read More</a>
        </div>

        <div class="card outline">
            <h2>Outline</h2>
            <p>Dark background with a bright cyan border.</p>
            <a href="#">Read More</a>
        </div>

    </div>

</body>
</html>
