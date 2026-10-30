<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Audit and Fixes</title>

    <style>
        * {
            box-sizing: border-box;
            margin: 0;
        }

        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            padding: 16px;
            background: #f4f6fb;
        }

        .container {
            width: 100%;
            max-width: 960px;
            margin: auto;
        }

        h1 {
            font-size: clamp(26px, 5vw, 45px);
            margin-bottom: 16px;
        }

        nav {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-bottom: 20px;
        }

        nav a {
            background: #1f3a93;
            color: white;
            text-decoration: none;
            padding: 12px 16px;
            border-radius: 6px;
            min-height: 44px;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 16px;
        }

        .card {
            background: white;
            padding: 16px;
            border-radius: 10px;
        }

        img {
            max-width: 100%;
            height: auto;
            display: block;
            border-radius: 8px;
        }

        .card h2 {
            margin-top: 10px;
        }

        
        .table-wrap {
            overflow-x: auto;
            margin-top: 24px;
            background: white;
        }

        table {
            border-collapse: collapse;
            width: 100%;
            min-width: 600px;
        }

        th, td {
            border: 1px solid #ddd;
            padding: 10px;
            text-align: left;
        }
    </style>
</head>

<body>

    <div class="container">

        <h1>Responsive Audit – Fixed</h1>

        <nav>
            <a href="#">Home</a>
            <a href="#">Services</a>
            <a href="#">Pricing</a>
            <a href="#">Blog</a>
            <a href="#">Contact</a>
        </nav>

        <div class="grid">

            <div class="card">
                <img src="https://picsum.photos/id/1011/800/500" alt="Boat on a lake">
                <h2>Card One</h2>
            </div>

            <div class="card">
                <img src="https://picsum.photos/id/1015/800/500" alt="Valley with a river">
                <h2>Card Two</h2>
            </div>

            <div class="card">
                <img src="https://picsum.photos/id/1016/800/500" alt="Rocky canyon">
                <h2>Card Three</h2>
            </div>

        </div>

        <div class="table">
            <table>
                <tr>
                    <th>Plan</th>
                    <th>Storage</th>
                    <th>Users</th>
                    <th>Support</th>
                    <th>Price</th>
                </tr>

                <tr>
                    <td>Basic</td>
                    <td>10 GB</td>
                    <td>1</td>
                    <td>Email</td>
                    <td>₹0</td>
                </tr>

                <tr>
                    <td>Pro</td>
                    <td>100 GB</td>
                    <td>5</td>
                    <td>Chat</td>
                    <td>₹499</td>
                </tr>
            </table>
        </div>

    </div>

</body>
</html>

