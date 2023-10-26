<nav class="navbar">
    <div class="logo">
        <img src="yugioh-logo.png" alt="Yu-Gi-Oh! Logo" class="yugioh-logo">
    </div>
    <ul class="nav-links">
        <li><a href="/">Home</a></li>
        <li><a href="/CardList">Card</a></li>
        <li><a href="/Event">Events</a></li>
        <li><a href="/About">Abouts</a></li>
    </ul>
</nav>

<style>
.navbar {
    background-color: lightblue;
    padding: 10px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.nav-links {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
}

.nav-links li {
    margin-right: 20px;
}

.nav-links a {
    text-decoration: none;
    color: black;
    font-family: 'Yu-Gi-Oh! Font', sans-serif;
    font-size: 18px;
}

.logo img {
    display: block;
    width: 100px; /* Adjust the width as needed */
    height: auto; /* Maintain aspect ratio */
}
</style>