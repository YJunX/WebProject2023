<!-- ImprovedSvelteComponent.svelte -->
<script>
    // JavaScript logic here
    let authorName = "Kazuki Takahashi";
    let authorDescription = `Kazuo Takahashi, known professionally as Kazuki Takahashi, was a Japanese manga artist. He made his serial manga debut in 1986, and is best known as the author of Yu-Gi-Oh!, published in Weekly Shōnen Jump from 1996 to 2004.`;
</script>

<main>
    <hr/>
    <div class="name-container">
        <h1>Author</h1>
    </div>
    <hr />
    <div class="right-container">
        <div class="image-left">
            <img src="creator.png" alt="Creator image" />
        </div>
        <div class="text">
            <h1>{authorName}</h1>
            <p>{authorDescription}</p>
        </div>
    </div>
    <hr />
    <div class="left-container">
        <div class="text">
            <h1>History</h1>
            <p>
                "Yu-Gi-Oh" (Japanese: Yu☆Gi☆Oh) is a comic created by Japanese
                cartoonist Kazuki Takahashi. It was serialized in "Weekly Shonen
                Jump" from September 30, 1996 to March 2004, with a total of 343
                chapters and a single volume. 38 episodes in total. The work
                became very popular after its release and has been adapted into
                a series of computer games, mobile games, card games, table
                games, TV animations, animated movies, light novels and other
                works.
            </p>
            <p>
                "Yu-Gi-Oh!" tells the story of Yugi Muto, a Japanese high school
                student with a humble personality but good at playing games, who
                meets the soul of the ancient Egyptian Pharaoh and grows up as a
                result. In the early stages of the plot, various games were used
                as themes, but in the later stages, it was mainly about card
                games. Subsequently, card games also became the theme of the
                "Yu-Gi-Oh!" series. After the serialization of the original work
                ended, V-Jump began to serialize "Yu-Gi-Oh! R", which was drawn
                by Akira Ito and supervised by Kazuki Takahashi. 
            </p>
            <p>
                "Yu-Gi-Oh!" has
                been adapted into two animated versions. The first one was
                broadcast from April 1998 to October of the same year, and the
                second animation was broadcast from 2000 to 2004. After the end,
                there are still a series of animation works that will continue
                to be launched. As of 2022, eleven animations have been
                launched. The card game "Yu-Gi-Oh Trading Card Game" adapted
                from it enjoys high popularity around the world. 
            </p>
            <p>
                The cumulative
                number of copies sold in 2011 exceeded 25.17 billion, and it was
                recognized by Guinness World Records as "the world's most sold
                trading card game" Card Game" was recognized by Guinness World
                Records in 2013 as "the largest trading card game competition
                with the largest number of participants."
            </p>
        </div>
        <div class="image-right">
            <img src="creator2.png" alt="Creator image" style="width: 730px; height: auto;"/>
        </div>
    </div>
    <hr />
    <div class="name-container">
        <h1>Animetions</h1>
    </div>
    <hr />
    <div class="left-container">
        <div class="image-left">
            <img src="yugioh_s2.png" alt="Creator image" style="width: 730px; height: auto;"/>
        </div>
        <div class="text">
            <h1>Yu-Gi-Oh! Duel Monsters</h1>
            <p>
                A shy high-school student named Yugi Moto receives the
                fragmented pieces of an Egyptian artifact, known as the
                Millennium Puzzle, from his grandfather. When Yugi reassembles
                the puzzle he is possessed by the 3,000-year-old spirit of an
                ancient pharaoh. Yugi and his friends Joey, Tea and Hondo
                protect the puzzle, which contains powerful secrets many people
                would like to possess.
            </p>
        </div>
    </div>
    <hr/>
    <div class="left-container">
        <div class="text">
            <h1>Yu-Gi-Oh GX</h1>
            <p>
                Yu-Gi-Oh! G/X is set a generation in the future. Jaden Yuki 
                and new friends he meets while studying at the Duel Academy go on missions,
                fight duels and use special powers to become the King of Games. Jaden's
                skills are impressive, but he has a lot to learn to master them.
            </p>
        </div>
        <div class="image-right">
            <img src="Yu-Gi-Oh!-GX.png" alt="Creator image" style="width: 730px; height: auto;"/>
        </div>
    </div>
    <hr/>
    <div class="left-container">
        <div class="image-left">
            <img src="5DS.png" alt="Creator image" style="width: 730px; height: 400px;"/>
        </div>
        <div class="text">
            <h1>Yu-Gi-Oh! 5D's</h1>
            <p>
                When his friend, Jack Atlas, steals his invention and card, the Stardust Dragon, 
                Yusei Fudo strives to reclaim his possessions. However, his quest evolves into 
                a mission to save the world.
            </p>
        </div>
    </div>
    <hr/>
    <div class="left-container">
        <div class="text">
            <h1>Yu-Gi-Oh GX</h1>
            <p>
                Yu-Gi-Oh! G/X is set a generation in the future. Jaden Yuki 
                and new friends he meets while studying at the Duel Academy go on missions,
                fight duels and use special powers to become the King of Games. Jaden's
                skills are impressive, but he has a lot to learn to master them.
            </p>
        </div>
        <div class="image-right">
            <img src="Yu-Gi-Oh!-GX.png" alt="Creator image" style="width: 730px; height: auto;"/>
        </div>
        
</main>

<style>
    /* Scoped CSS styles here */
    .left-container {
        display: flex;
        align-items: center;
    }

    /* Scoped CSS styles here */
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
