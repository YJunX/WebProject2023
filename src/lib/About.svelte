<!-- src/App.svelte -->
<script>
    // Sample card data
    let cards = [
        {
            name: 'Dark Magician',
            type: 'Spellcaster',
            level: 7,
            attack: 2500,
            defense: 2100
        },
        {
            name: 'Blue-Eyes White Dragon',
            type: 'Dragon',
            level: 8,
            attack: 3000,
            defense: 2500
        },
        // Add more card data as needed
    ];
</script>

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


<main>
    <h2>Latest Cards</h2>
    {#each cards as card}
        <div class="card">
            <h3>{card.name}</h3>
            <p>Type: {card.type}</p>
            <p>Level: {card.level}</p>
            <p>Attack: {card.attack}</p>
            <p>Defense: {card.defense}</p>
        </div>
    {/each}
</main>


