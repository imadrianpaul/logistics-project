<script>
    import Carousel from "svelte-carousel";

    const LogoBrands = [
        "/src/assets/techinasialogo.png",
        "/src/assets/yahoonewslogo.png",
        "/src/assets/thestraittimeslogo.png",
        "/src/assets/financialtimeslogo.png",
        "/src/assets/japaneselogo.png",
        "src/assets/topinsingaporelogo.png",
        "src/assets/lifestyleasialoguelogo.png",
        "src/assets/suratkhabarsportslogo.png",
        "src/assets/heartofmalaysia.png",
        "src/assets/malaysiacornerlogo.png",
        "src/assets/bestinsingaporelogo.png",
        "src/assets/moneysmartlogo.png",
        "src/assets/asiaonelogo.png"
    ];

    // Function to chunk LogoBrands into groups of 3 logos
    const chunkedLogoBrands = [];
    for (let i = 0; i < LogoBrands.length; i += 3) {
        chunkedLogoBrands.push(LogoBrands.slice(i, i + 3));
    }
</script>

<div class="carousel-section">
    <h1>Featured On</h1>

    <!-- svelte-carousel component -->
    <Carousel
        autoplay={true}
        autoplayDuration={3000}
        duration={1000}
        timingFunction="ease-in-out"
        dots={false}
        arrows={false}
        swiping={true}
        class="carousel-container"
    >
        {#each chunkedLogoBrands as logoGroup}
        <div class="carousel-slide">
            {#each logoGroup as logo}
                <img src={logo} alt="Brand Logo" class="logo-brand" />
            {/each}
        </div>
        {/each}
    </Carousel>
</div>

<style>
    .carousel-section {


        text-align: center;
        height: 450px;
    }

    .carousel-container {

        display: flex;
        gap: 2rem;

    }

    .carousel-slide {

        display: flex;
        gap: 2rem;
        justify-content: center;
        margin-bottom: 2rem;
        padding-bottom: 2rem;

    }

    .logo-brand {
        height: 400px;
        width: 400px;
        object-fit: contain;
    }

    h1 {
        font-size: 2rem;
        color: #fea238;
        text-transform: uppercase;
        margin-top: 4rem;
        margin-bottom: 3rem;
    }
</style>
