<!-- Footer Section -->
<div class="footer">
  <!-- Logo and Information Container -->
  <div class="footer-logo-container">
    <img src="yugioh-logo.png" alt="Logo" class="footer-logo" />
    <!-- Information List -->
    <div class="informations-list">
      <p>Welcome to play yugiog together</p>
    </div>
  </div>
   <!-- Navigation Links Container -->
  <div class="footer-link">
    <!-- Information Container for Navigation Links -->
    <div class="info-container">
      <div class="column">
        <!-- Column 1: Home and Card List Links -->
        <div class="Home">
          <h3><a href="/">Home</a></h3>
      
        </div>

        <div class="Cardlist">
          <h3><a href="/CardList">Card</a></h3>
       
        </div>
      </div>

      <div class="column">
        <div class="Tournaments">
          <h3><a href="/Tournaments">Tournaments</a></h3>
        
        </div>

        <div class="About">
          <h3><a href="/About">About</a></h3>
          
        </div>
      </div>
    </div>
  </div>
  <div class="copyright">
    <p>&copy; 2023 Yu-Gi-Oh, inc.</p>
  </div>
</div>

<style>
  .footer {
    background-color: #161616;
    margin-top: auto;
  }


  .footer-logo-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin-bottom: 10px;
  }
  .footer-link  {
    list-style-type: none;
    margin: 0;
    padding: 0;
    text-align: center;
}

/* Style the navigation links */
.footer-link a {
    text-decoration: none;
    color: #FFD700; /* Gold color */
}

.footer-link a:hover {
    color: #FFFFFF; /* White color */
}
  .footer-logo {
    width: 100px;
  }

  .info-container {
    display: flex;
    justify-content: space-between;
    margin-bottom: 10px;
  }

  .column {
    display: flex;
    flex-direction: column;
    flex: 1;
  }

  .informations-list {
    display: flex;
    flex-direction: column;
    text-align: left;
  }

  .informations-list p {
    margin: 5px 0;
    color: white;
  }

  .copyright {
    font-size: smaller;
    max-width: 100%;
    margin-top: 50px;
    text-align: center;
  }
  .copyright p {
    margin: 0;
  }
</style>
