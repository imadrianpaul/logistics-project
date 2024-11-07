<!-- <script>
    import Carousel from "svelte-carousel";
    import "svelte-carousel/src/svelte-carousel.css";

</script>

<Carousel
  autoplay={true}
  autoplayDuration={0}
  duration={5000} 
  timingFunction="linear"
  dots={false}
  arrows={false}
  swiping={false}
  class="carousel-container"
>

    {#each LogoBrands as logo (logo)}
        <img src={logo} alt="Brand Logo" class="logo-brand" />
    {/each}

</Carousel>


<style>
    .carousel-container {
        display: flex;
        overflow: hidden;
        flex-wrap: nowrap;
        gap: 2rem;
    }

    .logo-brand {
        width: 150px;
        height: auto;
        object-fit: contain;
    }

    .svelte-carousel {
        display: flex;
        align-items: center;
    }
</style> -->
