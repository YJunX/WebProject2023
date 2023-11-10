<script>
    // Initialize variables to store card name and data
    let cardName = "";
    let cardData = [];

    // Async function to search for cards based on the entered card name
    async function searchCards() {
        // Fetch card data from the API based on the provided card name
        const response = await fetch(
            `https://db.ygoprodeck.com/api/v7/cardinfo.php?name=${cardName}`
        );
        // Parse the response JSON and store data in the cardData variable
        const data = await response.json();
        cardData = data.data;
    }

    // Async function to get all cards from the API
    async function getAllCards() {
        // Fetch all card data from the API
        const response = await fetch(
            'https://db.ygoprodeck.com/api/v7/cardinfo.php'
        );
        // Parse the response JSON and store data in the cardData variable
        const data = await response.json();
        cardData = data.data;
    }
</script>

<!-- HTML content -->
<h1>Yu-Gi-Oh! Card List</h1>

<!-- Input field for entering card name, with two buttons for searching and showing all cards -->
<input type="text" bind:value={cardName} placeholder="Enter card name" />
<button on:click={searchCards}>Search</button>
<button on:click={getAllCards}>Show All Cards</button>

<!-- Container for displaying cards -->
<div class="card-container">
    <!-- Check if there are cards in the cardData array -->
    {#if cardData.length > 0}
        <!-- Loop through each card in the cardData array -->
        {#each cardData as card}
            <div class="card">
                <!-- Display card image with alt text -->
                <img class="card-image" src={card.card_images[0].image_url} alt={card.name} />
                <!-- Display card details, such as name, type, attack, and defense -->
                <div class="card-details">
                    <b>Name:</b> {card.name}<br />
                    <b>Type:</b> {card.type}<br />
                    <!-- Display attack if available -->
                    {#if card.atk !== undefined}
                        <b>Attack:</b> {card.atk}<br />
                    {/if}
                    <!-- Display defense if available -->
                    {#if card.def !== undefined}
                        <b>Defense:</b> {card.def}<br />
                    {/if}
                </div>
            </div>
        {/each}
    <!-- If no cards are found, display a message -->
    {:else}
        <p>No cards found.</p>
    {/if}
</div>







