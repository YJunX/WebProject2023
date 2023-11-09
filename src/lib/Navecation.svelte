<nav class="navbar">
    <div class="logo">
        <img src="yugioh-logo.png" alt="Yu-Gi-Oh! Logo" class="yugioh-logo">
    </div>
    <hr/>
    <ul class="nav-link">
        <li><a href="/">Home</a></li>
        <li><a href="/CardList">Card List</a></li>
        <li><a href="/About">Abouts</a></li>
        <li class="dropdown">
            <a href="/Tournaments">Tournaments</a>
            <div class="dropdown-content">
                <a href="/">Past Tournaments</a>
                <a href="/">Rules</a>
                <a href="/">Shop</a>
            </div>
        </li>
    </ul>
</nav>

<style>
.navbar {
    background-color: #161616; /* Dark background color */
    padding: 10px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.nav-link {
    list-style-type: none;
    margin: 0;
    padding: 0;
    text-align: center;
}

.nav-link li {
    display: inline;
    margin-right: 20px;
    font-size: 18px;
    font-weight: bold;
}

/* Style the navigation links */
.nav-link a {
    text-decoration: none;
    color: #FFD700; /* Gold color */
}

/* Change link color on hover */
.nav-link a:hover {
    color: #FFFFFF; /* White color */
}

.yugioh-logo {
    max-width: 100px; /* Adjust the value to make the logo smaller as needed */
    height: auto; /* This will maintain the aspect ratio */
}

/* Style the dropdown menu */
.dropdown {
    position: relative;
    display: inline-block;
}

/* Style the dropdown content */
.dropdown-content {
    display: none;
    position: absolute;
    background-color: #161616;
    min-width: 200px;
    z-index: 1;
    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
    top: 100%; /* Position the dropdown below the parent link */
    left: 0; /* Align the left edge of the dropdown with the parent link */
}

/* Style the dropdown links */
.dropdown-content a {
    color: #FFD700;
    padding: 12px 16px;
    display: block;
    text-align: left;
    text-decoration: none;
}

/* Change link color on hover in the dropdown */
.dropdown-content a:hover {
    color: #FFFFFF;
}

/* Show the dropdown content when hovering over the dropdown */
.dropdown:hover .dropdown-content {
    display: block;
}

</style>