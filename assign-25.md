styled-multipage-project.html

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Styled multi-page project">
    <title>My Website</title>

    <style>
        :root {
            --primary: #1f3a93;
            --accent: orange;
            --bg: #f5f5f5;
        }

        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: var(--bg);
            color: #222;
        }

        header {
            background: var(--primary);
            color: white;
            padding: 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 5px;
        }

        nav a:hover {
            color: var(--accent);
        }

        main {
            max-width: 800px;
            margin: auto;
            padding: 20px;
        }

        .page {
            display: none;
            background: white;
            padding: 20px;
            border-radius: 8px;
        }

        .page:target,
        body:not(:has(.page:target)) #home {
            display: block;
        }

        h2 {
            color: var(--primary);
        }

        label {
            display: block;
            margin-bottom: 15px;
        }

        input, select, textarea {
            display: block;
            width: 100%;
            padding: 8px;
            margin-top: 5px;
            box-sizing: border-box;
        }

        button {
            background: var(--accent);
            border: none;
            padding: 10px 20px;
            cursor: pointer;
        }

        table {
            width: 100%;
            border-collapse: collapse;
        }

        th, td {
            border: 1px solid #ccc;
            padding: 10px;
            text-align: left;
        }

        .note {
            background: #fff8ec;
            padding: 15px;
            border-left: 5px solid var(--accent);
        }

        footer {
            text-align: center;
            padding: 15px;
        }
    </style>
</head>

<body>

    <header>
        <h1>Anushkaaa's Site</h1>

        <nav>
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#register">Register</a>
            <a href="#contact">Contact</a>
            <a href="#design">Design Note</a>
        </nav>
    </header>

    <main>

        <section id="home" class="page">
            <h2>Home</h2>
            <p>Welcome to my styled multi-page website!</p>
        </section>

        <section id="about" class="page">
            <h2>About</h2>

            <table>
                <tr>
                    <th>City</th>
                    <td>Bareilly , UP</td>
                </tr>
                <tr>
                    <th>Course</th>
                    <td>BCA-AI</td>
                </tr>
                <tr>
                    <th>Interests</th>
                    <td>Music,Dance,Movies</td>
                </tr>
            </table>
        </section>

        <section id="register" class="page">
            <h2>Registration</h2>

            <form>
                <p>Name:<input type="text" name="name" placeholder="enter your name here"></p>
                <p>Email:<input type="email" name="email" placeholder="enter your name here"></p>
                Course:
                    <select>
                        <option>BCA-AI</option>
                        <option>B.Tech</option>
                    </select>

                <button type="submit">Register</button>
            </form>
        </section>

        <section id="contact" class="page">
            <h2>Contact</h2>

            <form>
                <p>Name:<input type="text" name="name" placeholder="enter your name here"></p>
                Message<textarea rows="4"placeholder="enter your message here"></textarea>
                <button type="submit">Send</button>
            </form>
        </section>

        <section id="design" class="page">
            <h2>Design Choices</h2>

            <div class="note">
                <p><strong>Colour:</strong> Blue gives a professional look, while orange highlights buttons.</p>

                <p><strong>Font:</strong> Arial makes the text easy to read.</p>

                <p><strong>Layout:</strong> The content is centered on the page with a white background.</p>

                <p><strong>CSS Variables:</strong> Colours can be changed easily in one place.</p>
            </div>
        </section>

    </main>

    <footer>
        <small>&copy; 2026 Anushka Mishra</small>
    </footer>

</body>
</html>

