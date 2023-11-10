<script>
    // Initialize variables for author information
    let authorName = "Kazuki Takahashi";
    let authorDescription = `Kazuo Takahashi, known professionally as Kazuki Takahashi, was a Japanese manga artist. He made his serial manga debut in 1986, and is best known as the author of Yu-Gi-Oh!, published in Weekly Shōnen Jump from 1996 to 2004.`;
</script>

<!-- Main content section -->
<main>
    <!-- Horizontal line -->
    <hr />

    <!-- Container for author name -->
    <div class="name-container">
        <h1>Author</h1>
    </div>

 
    <hr />

    <!-- Right container for author information -->
    <div class="right-container">
        <!-- Left side with author image -->
        <div class="image-left">
            <img src="creator.png" alt="Creator image" />
        </div>
        <!-- Right side with author name and description -->
        <div class="text">
            <h1>{authorName}</h1>
            <p>{authorDescription}</p>
        </div>
    </div>

  
    <hr />

    <!-- Left container for history section -->
    <div class="left-container">
        <!-- Text content -->
        <div class="text">
            <h1>History</h1>
            <!-- Paragraphs providing information about the history of "Yu-Gi-Oh!" -->
            <!-- Each paragraph describes different aspects of the manga and its adaptations -->
        </div>
        <!-- Right side with an image -->
        <div class="image-right">
            <img src="creator2.png" alt="Creator image" style="width: 730px; height: auto;" />
        </div>
    </div>


    <hr />

    <!-- Container for the section name "Animations" -->
    <div class="name-container">
        <h1>Animations</h1>
    </div>


    <hr />

    <!-- Left container for "Yu-Gi-Oh! Duel Monsters" -->
    <div class="left-container">
        <!-- Left side with an image -->
        <div class="image-left">
            <img src="yugioh_s2.png" alt="Creator image" style="width: 730px; height: auto;" />
        </div>
        <!-- Right side with text content -->
        <div class="text">
            <h1>Yu-Gi-Oh! Duel Monsters</h1>
            <!-- Paragraph providing information about the "Yu-Gi-Oh! Duel Monsters" animation -->
        </div>
    </div>


    <hr />

    <!-- Left container for "Yu-Gi-Oh! GX" -->
    <div class="left-container">
        <!-- Text content -->
        <div class="text">
            <h1>Yu-Gi-Oh GX</h1>
            <!-- Paragraph providing information about the "Yu-Gi-Oh! GX" animation -->
        </div>
        <!-- Right side with an image -->
        <div class="image-right">
            <img src="Yu-Gi-Oh!-GX.png" alt="Creator image" style="width: 730px; height: auto;" />
        </div>
    </div>


    <hr />

    <!-- Left container for "Yu-Gi-Oh! 5D's" -->
    <div class="left-container">
        <!-- Left side with an image -->
        <div class="image-left">
            <img src="5DS.png" alt="Creator image" style="width: 730px; height: 400px;" />
        </div>
        <!-- Right side with text content -->
        <div class="text">
            <h1>Yu-Gi-Oh! 5D's</h1>
            <!-- Paragraph providing information about the "Yu-Gi-Oh! 5D's" animation -->
        </div>
    </div>


    <hr />

    <!-- Left container for "Yu-Gi-Oh! Zexal" -->
    <div class="left-container">
        <!-- Text content -->
        <div class="text">
            <h1>Yu-Gi-Oh! Zexal</h1>
            <!-- Paragraph providing information about the "Yu-Gi-Oh! Zexal" animation -->
        </div>
        <!-- Right side with an image -->
        <div class="image-right">
            <img src="yugioh-zx.png" alt="Creator image" style="width: 730px; height: 400px;" />
        </div>
    </div>
</main>

<!-- Scoped CSS styles -->
<style>
    /* Scoped CSS styles for adjusting layout and appearance */
    .left-container {
        display: flex;
        align-items: center;
    }

    .right-container {
        display: flex;
        align-items: center;
    }

    .name-container {
        display: flex;
        justify-content: center; /* Center the content horizontally */
        align-items: center; /* Center the content vertically */
        text-align: center; /* Center the text within the container */
    }

    .image-left {
        margin-right: 20px; /* Adjust margin to create space between image and text */
    }

    .image-right {
        margin-left: 20px; /* Adjust margin to create space between text and image */
    }

    .text {
        flex: 1;
    }
</style>
