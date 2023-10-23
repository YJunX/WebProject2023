<!-- src/App.svelte -->
<script>
    import { onMount } from "svelte";

    // Define an array to store the card data from the API
    let Cards = [];

    // Function to fetch card data from the API
    async function fetchCardData() {
        try {
            const response = await fetch(
                "https://db.ygoprodeck.com/api/v7/cardinfo.php"
            );
            if (response.ok) {
                const data = await response.json();
                // Assuming the API response is an array of cards
                Cards = data.data;
            } else {
                console.error("Failed to fetch data from the API");
            }
        } catch (error) {
            console.error("Error:", error);
        }
    }

    // Fetch card data when the component is mounted
    onMount(fetchCardData);
</script>

<main>
    <h2>Latest Cards</h2>
    {#each Cards as card (card.id)}
        <!-- Assuming each card has a unique ID -->
        <div class="card">
            <h3>{card.name}</h3>
            <p>Type: {card.type}</p>
            <p>Level: {card.level}</p>
            <p>Attack: {card.attack}</p>
            <p>Defense: {card.defense}</p>
        </div>
    {/each}
</main>

<style>
    /* Add your CSS styles here */
    /* Example: style the cards */
    .card {
        border: 1px solid #ccc;
        padding: 10px;
        margin: 10px;
        border-radius: 5px;
    }
</style>
