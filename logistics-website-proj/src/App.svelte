<script>
    import Navbar from './layouts/Navbar.svelte';
    import Home from './pages/Home.svelte';
</script>

<main>
  <div class="home-page">
    <Navbar />
    <Home />
  </div>
</main>

<style>
  main {
    justify-content: center;
  }

  .home-page {

    margin: 0 auto;
  }
</style>

