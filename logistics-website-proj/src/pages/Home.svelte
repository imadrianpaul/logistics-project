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
    <div>
        <SDFSection />
    </div>
    <div class="guide-wrapper">
        <GuideSection />
        <div class="bg-filter2"></div>
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

</style>