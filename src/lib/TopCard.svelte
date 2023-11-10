<!-- src/App.svelte -->
<script>
    import { onMount } from "svelte";

    // Define an array to store the card data
    let cards = [];
    let cardNames = [
        "Dark Magician",
        "Blue-Eyes White Dragon",
        "Elemental HERO Neos",
        "Number 39: Utopia",
        "Stardust Dragon", 
        "Odd-Eyes Pendulum Dragon",
        "Decode Talker",
        "Firewall Dragon",
        
    ]; // Default card names

    // Function to fetch card data from the API by names
    async function fetchCardData() {
        try {
            const cardPromises = cardNames.map(async (name) => {
                const response = await fetch(
                    `https://db.ygoprodeck.com/api/v7/cardinfo.php?name=${encodeURIComponent(
                        name
                    )}`
                );
                if (response.ok) {
                    const data = await response.json();
                    if (data.data.length > 0) {
                        return data.data[0]; // Use the first card
                    } else {
                        console.error(`Card '${name}' not found`);
                        return null;
                    }
                } else {
                    console.error(
                        `Failed to fetch data for '${name}' from the API`
                    );
                    return null;
                }
            });

            cards = await Promise.all(cardPromises);
        } catch (error) {
            console.error("Error:", error);
        }
    }

    // Fetch card data when the component is mounted
    onMount(fetchCardData);
</script>

<main>
    <h2>All protagonist cards, main monsters</h2>
        <div class="card-container">
            {#each cards as card (card.id)}
                <!-- Assuming each card has a unique ID -->
                <div class="card">
                    <img src={card.card_images[0].image_url} alt={card.name} />
                    <h3>{card.name}</h3>
                    <p>Type: {card.type}</p>
                    <p>Attack: {card.atk}</p>
                    <!-- Use 'atk' instead of 'attack' as per the API response -->
                </div>
            {/each}
        </div>
</main>

<style>
    /* Add your CSS styles here */
    .card-container {
        display: flex; /* Display cards side by side */
        flex-wrap: wrap; /* Allow cards to wrap to the next line */
    }

    .card {
        border: 1px solid #ccc;
        padding: 10px;
        margin: 10px;
        border-radius: 5px;
        max-width: 300px; /* Set the maximum width to your desired size */
        flex: 0 0 calc(33.333% - 20px); /* 3 cards per line with spacing */
    }

    .card img {
        width: 100%; /* Use 100% width for responsiveness */
        display: block;
        margin-top: 10px;
    }
</style>
