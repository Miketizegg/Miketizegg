<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Arch Alibaba</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="background-images"></div> <!-- Background images container -->

    <header>
        <!-- Header content: Logo, Search bar, User authentication -->
    </header>

    <nav>
        <!-- Navigation content: Categories, Auction, Contact -->
    </nav>

    <main>
        <section id="home">
            <!-- Home section content: Featured designs, New arrivals -->
        </section>

        <section id="designs">
            <!-- Designs section content: Architectural designs listings -->
        </section>

        <section id="auction">
            <!-- Auction section content: Designs available for auction -->
        </section>

        <section id="contact">
            <!-- Contact section content: Messaging system -->
        </section>
    </main>

    <footer>
        <!-- Footer content: Links, About, Contact -->
    </footer>

    <script src="script.js"></script>
</body>
</html>
/* Global Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

/* Background Images */
.background-images {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
    background-image: url('building1.jpg'), url('building2.jpg'), url('building3.jpg');
    background-size: cover;
    background-position: center;
    filter: blur(8px); /* Add a slight blur effect for a more subtle background */
}

header {
    background-color: #fff;
    padding: 20px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

nav {
    background-color: #f3f3f3;
    padding: 10px 20px;
}

nav ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
}

nav ul li {
    display: inline;
    margin-right: 20px;
}

nav ul li a {
    text-decoration: none;
    color: #333;
}

main {
    padding: 20px;
}

footer {
    background-color: #f3f3f3;
    padding: 20px;
    text-align: center;
}
// JavaScript code goes here

document.addEventListener("DOMContentLoaded", function() {
    // Prevent right-click on the entire document
    document.addEventListener("contextmenu", function(e) {
        e.preventDefault();
    });

    // Disable specific keyboard shortcuts
    document.addEventListener("keydown", function(e) {
        if ((e.ctrlKey || e.metaKey) && (e.key === "c" || e.key === "x" || e.key === "v" || e.key === "a" || e.key === "p" || e.key === "s" || e.key === "j")) {
            e.preventDefault();
        }
    });
});
