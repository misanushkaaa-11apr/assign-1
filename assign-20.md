<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Multi-page HTML project: Home, About, Registration and Contact.">
    <meta name="author" content="Anushka Mishra">
    <title>Multi-Page Project</title>

    <style>
      *{
        background-color: #c57956fe;
      }
      body {
        font-family: Arial, sans-serif;
        max-width: 760px;
        margin: auto;
        padding: 15px;
      }
      .page {
        display: none;
      }
      .page:target,
      body:not(:has(.page:target)) #home {
        display: block;
      }
    </style>
</head>

<body>

    <header>
        <h1>Anushka's Website</h1>

        <nav>
            <a href="#home">Home</a> |
            <a href="#about">About</a> |
            <a href="#registration">Registration</a> |
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <main>

        <section id="home" class="page">
            <h2>Home</h2>
            <p>Welcome to my website!</p>

            <img src="https://images4.alphacoders.com/807/thumb-1920-807156.jpg"alt="Mountain landscape"
                 width="600">

            <h3>What You Can Do:-</h3>
            <ul>
                <li><a href="#about">Read About Me</a></li>
                <li><a href="#registration">Register for Workshop</a></li>
                <li><a href="#contact">Contact Me</a></li>
            </ul>
        </section>

        <section id="about" class="page">
            <h2>About Me</h2>
            <p>I am a BCA-AI student HTML & CSS.</p>

            <table border="1" cellpadding="6">
                <tr>
                    <th>City</th>
                    <td>Bareilly,UP</td>
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

       <section id="registration" class="page">
            <h2>Registration</h2>

            <form>
                <p>Name:<input type="text" name="name" placeholder="enter your name here"></p>
                <p>Email:<input type="email" name="email" placeholder="enter your name here"></p>
                <p>Date of Birth:<input type="date"></p>
                <p>
                    Level:
                    <select>
                        <option>Beginner</option>
                        <option>Intermediate</option>
                    </select>
                </p>

                <button type="submit">Register</button>
            </form>
        </section>

        <section id="contact" class="page">
            <h2>Contact Me</h2>

            <form>
                <p>Your Name:<input type="text" name="name" placeholder="enter your name here"></p>
                <p>
                    Message:
                    <br>
                    <textarea rows="5" cols="30" required></textarea>
                </p>

                <button type="submit">Send</button>
            </form>

            <p>Email:misanushkaaa@gmail.com</p>
        </section>

    </main>

    <footer>
        <hr>
        <p>&copy; 2026 Anushka Mishra</p>
    </footer>

</body>
</html>
