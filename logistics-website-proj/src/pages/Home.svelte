<script>
    import HeroSection from "./Home/HeroSection.svelte";
    import SDFSection from "./Home/SDFSection.svelte";
    import GuideSection from "./Home/GuideSection.svelte";
    import CarouselF from "./Home/CarouselF.svelte";
</script>

<div class="home-container">
    <div class="hero-wrapper">
        <HeroSection />
        <div class="bg-filter"></div>
    </div>
    <div class="services-wrapper">
        <div>
        <SDFSection />
        <img src="/src/assets/box1.PNG" alt="Box Image" class="box-image">
        <img src="/src/assets/box2.PNG" alt="Box Image" class="box-image2">
        <img src="/src/assets/box3.PNG" alt="Box Image" class="box-image3">
        </div>

    </div>
    <div class="guide-wrapper">
        <GuideSection />
        <div class="bg-filter2"></div>
    </div>
    <div class="carousel-wrapper">
        <CarouselF />
        <img src="/src/assets/box4.PNG" alt="Box Image" class="box-image4">
    </div>
</div>

<style>
    .home-container {
        width: 100%;
        margin: 0 auto;
    }

    .hero-wrapper {
        position: relative;
        background-image: url('/src/assets/hero-image.jpg');
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
        height: 100vh;
        width: auto;
    }
    
    .bg-filter {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background-color: rgba(0, 0, 0, 0.4);
        z-index: 1; 
    }

    .services-wrapper { 

        position: relative;
        padding: 20px;
    }

    .box-image {

        position: absolute;
        left: 15%;
        top: 6.5%;
        transform: translateY(-50%);
        width: 341px;
        height: 145px;
        background-size: contain;
        background-repeat: no-repeat;
        opacity: 0.25;
        z-index: 0;
        pointer-events: none;

    }

    .box-image2 {

        position: absolute;
        right: 60%;
        top: 65%;
        transform: translateY(-50%);
        width: 341px;
        height: 145px;
        background-size: contain;
        background-repeat: no-repeat;
        opacity: 0.25;
        z-index: 0;
        pointer-events: none;

    }

    .box-image3 {

        position: absolute;
        right: 5%;
        top: 33%;
        transform: translateY(-50%);
        width: 275px;
        height: 300px;
        background-size: contain;
        background-repeat: no-repeat;
        opacity: 0.25;
        z-index: 0;
        pointer-events: none;

    }

    .box-image4 {

        position: absolute;
        left: 20%;
        top: 20%;
        transform: translateY(-50%);
        width: 341px;
        height: 175px;
        background-size: contain;
        background-repeat: no-repeat;
        opacity: 0.25;
        z-index: 0;
        pointer-events: none;

    }

    .guide-wrapper {
        position: relative;
        background-image: url('/src/assets/guide-image.jpg');
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
        width: auto;
    }

    .bg-filter2 {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background-color: rgb(0, 0, 0, 0.6);
        z-index: 1;
    }

    .carousel-wrapper {

        position: relative;
        padding: 20px;
    }

</style>