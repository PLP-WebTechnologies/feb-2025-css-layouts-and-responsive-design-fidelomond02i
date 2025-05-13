# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.


HTML:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Navigation</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <nav>
        <h1>My Website</h1>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
    <main>
        <h2 id="home">Home</h2>
        <p>Welcome to my website!</p>
        <h2 id="about">About</h2>
        <p>Learn more about me and my work.</p>
        <h2 id="services">Services</h2>
        <p>Check out the services I offer.</p>
        <h2 id="contact">Contact</h2>
        <form>
            <label for="name">Name:</label>
            <input type="text" id="name" name="name">
            <label for="email">Email:</label>
            <input type="email" id="email" name="email">
            <input type="submit" value="Send">
        </form>
    </main>
</body>
</html>
CSS (styles.css):
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
}

body {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
}

nav {
    background-color: #333;
    color: #fff;
    padding: 1em 0;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
    display: flex;
    justify-content: space-around;
}

nav li {
    margin: 0 1em;
}

nav a {
    display: block;
    color: #fff;
    text-decoration: none;
    padding: 0.5em 1em;
    text-align: center;
}

main {
    flex: 1;
    padding: 2em;
    text-align: center;
}

@media (max-width: 768px) {
    nav {
        flex-direction: column;
    }

    nav ul {
        justify-content: center;
    }

    nav a {
        margin: 0.5em 0;
    }

    main {
        text-align: left;
    }
}
Happy Coding! 💻✨
