<script>
    let cardName = "";
    let cardData = [];

    async function searchCards() {
        const response = await fetch(
            `https://db.ygoprodeck.com/api/v7/cardinfo.php?name=${cardName}`
        );
        const data = await response.json();
        cardData = data.data;
    }

    async function getAllCards() {
        const response = await fetch(
            'https://db.ygoprodeck.com/api/v7/cardinfo.php'
        );
        const data = await response.json();
        cardData = data.data;
    }
</script>

<h1>Yu-Gi-Oh! Card List</h1>

<input type="text" bind:value={cardName} placeholder="Enter card name" />
<button on:click={searchCards}>Search</button>
<button on:click={getAllCards}>Show All Cards</button>

<div class="card-container">
    {#if cardData.length > 0}
        {#each cardData as card}
            <div class="card">
                <img class="card-image" src={card.card_images[0].image_url} alt={card.name} />
                <div class="card-details">
                    <b>Name:</b> {card.name}<br />
                    <b>Type:</b> {card.type}<br />
                    {#if card.atk !== undefined}
                        <b>Attack:</b> {card.atk}<br />
                    {/if}
                    {#if card.def !== undefined}
                        <b>Defense:</b> {card.def}<br />
                    {/if}
                </div>
            </div>
        {/each}
    {:else}
        <p>No cards found.</p>
    {/if}
</div>

<style>
    h1 {
        font-size: 24px;
        color: #333;
    }

    input {
        padding: 8px;
        font-size: 16px;
    }

    button {
        background-color: #0077cc;
        color: #fff;
        padding: 8px 16px;
        border: none;
        cursor: pointer;
        margin-right: 10px;
    }

    .card-container {
        display: flex;
        flex-wrap: wrap;
    }

    .card {
        border: 1px solid #ddd;
        padding: 8px;
        margin: 8px;
        display: flex;
        width: calc(33.33% - 16px); /* Adjust the width as needed */
    }

    .card-image {
        width: 100px; /* Adjust the width as needed */
        height: auto; /* Maintain aspect ratio */
        margin-right: 10px;
    }

    .card-details {
        flex: 1;
    }
</style>
