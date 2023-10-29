<!-- ImprovedSvelteComponent.svelte -->
<script>
    // JavaScript logic here
    let authorName = "Kazuki Takahashi";
    let authorDescription = `Kazuo Takahashi, known professionally as Kazuki Takahashi, was a Japanese manga artist. He made his serial manga debut in 1986, and is best known as the author of Yu-Gi-Oh!, published in Weekly Shōnen Jump from 1996 to 2004.`;
</script>

<main>
    <div class="about-container">
        <div class="image-left">
            <img src="creator.png" alt="Creator image" />
        </div>
        <div class="text">
            <h1>{authorName}</h1>
            <p>{authorDescription}</p>
        </div>
    </div>
    <div class="history-container">
        <div class="image-right">
            <img src="creator2.png" alt="Creator image" />
        </div>
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
                by Akira Ito and supervised by Kazuki Takahashi. "Yu-Gi-Oh!" has
                been adapted into two animated versions. The first one was
                broadcast from April 1998 to October of the same year, and the
                second animation was broadcast from 2000 to 2004. After the end,
                there are still a series of animation works that will continue
                to be launched. As of 2022, eleven animations have been
                launched. The card game "Yu-Gi-Oh Trading Card Game" adapted
                from it enjoys high popularity around the world. The cumulative
                number of copies sold in 2011 exceeded 25.17 billion, and it was
                recognized by Guinness World Records as "the world's most sold
                trading card game" Card Game" was recognized by Guinness World
                Records in 2013 as "the largest trading card game competition
                with the largest number of participants."
            </p>
        </div>
    </div>
</main>

<style>
    /* Scoped CSS styles here */
    .about-container {
        display: flex;
        align-items: center;
    }

    .image-left {
        margin-right: 20px; /* Adjust margin to create space between image and text */
    }

    .image-right {
        margin-right: 20px;
    }

    .text {
        flex: 1;
    }
</style>
