<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Fixing overflow that breaks a layout.">
    <title>Fixing Overflow Problems</title>

    <style>
        * {
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 15px;
        }

        .wrapper {
            max-width: 700px;
            margin: auto;
        }

        .column {
            width: 100%;
            padding: 15px;
            border: 2px solid #1d3557;
            margin-bottom: 15px;
            background: white;
        }

        img {
            max-width: 100%;
            height: auto;
        }

        .long-text {
            overflow-wrap: anywhere;
        }

        .table-scroll {
            overflow-x: auto;
        }

        .fixed-box {
            height: 90px;
            overflow-y: auto;
            border: 1px solid gray;
            padding: 10px;
        }

        pre {
            overflow-x: auto;
            background: #eee;
            padding: 10px;
        }
    </style>
</head>

<body>

    <div class="wrapper">

        <h1>Overflow Problems and Solutions</h1>

        <div class="column">
            <h2>1. Image Overflow</h2>
            <img src="https://picsum.photos/id/1011/1000/400"
                 alt="A rower on a calm lake">
        </div>

        <div class="column long-text">
            <h2>2. Long Text</h2>
            <p>
                https://www.example.com/this/is/a/very/long/url/that/would/stretch/the/layout
            </p>
        </div>

        <div class="column">
            <h2>3. Wide Table</h2>

            <div class="table-scroll">
                <table border="3">
                    <tr>
                        <th>ID</th>
                        <th>Name</th>
                        <th>Email</th>
                        <th>City</th>
                        <th>Course</th>
                        <th>Year</th>
                    </tr>
                    <tr>
                        <td>1</td>
                        <td>Anushka</td>
                        <td>misanushkaaa@gmail.com</td>
                        <td>Bareilly</td>
                        <td>BCA-AI</td>
                        <td>2026</td>
                    </tr>
                </table>
            </div>
        </div>

        <div class="column">
            <h2>4. Fixed-Height Box</h2>

            <div class="fixed-box">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Sed do eiusmod tempor incididunt ut labore et dolore magna
                aliqua. Ut enim ad minim veniam, quis nostrud exercitation
                ullamco laboris nisi ut aliquip ex ea commodo consequat.
            </div>
        </div>

        <div class="column">
            <h2>5. Code Block</h2>

            <pre>const message = "This is a very long line of code that may overflow";</pre>
        </div>

    </div>

</body>
</html>
