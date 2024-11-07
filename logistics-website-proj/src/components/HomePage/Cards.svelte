<script>
    export let title = "";
    export let subtitle = "";
    export let description = "";
    export let description2 = "";
</script>

<div class="card">
    <div class="card-content">
        <h2 class="card-title">{title}</h2>
        <h3 class="card-subtitle">{subtitle}</h3>
        <p class="card-description">{description}</p>
        <p class="card-description2">{description2}</p>
        <slot name="actions"></slot>
    </div>
</div>

<style>
    
    .card {
        max-width: 300px;
        height: 400px;
        border-radius: 20px;
        overflow: hidden;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);  
        background: linear-gradient(to top, rgba(255, 223, 167, 0.25), rgba(254, 162, 56, 0.75));
        transition: transform 0.2s;
    }

    .card:hover {
        transform: translateY(-5px);
    }

    .card-content {

        margin-top: 1rem;
        padding: 1rem;

    }

    .card-title {
        font-size: 24px;
        margin: 0.5rem 0;
        color: #ffffff;
    }

    .card-subtitle {

        color: #fff;
        font-size: 24px;
    }

    .card-description {
        font-size: 16px;
        font-family: Inter, sans-serif;
        color: #666;
        margin: 2rem 0 0 0;
        padding: 2rem 0 0 0;
        height: 50px;
    }

    .card-description2 {
        font-size: 0.9rem;
        color: #666;
        margin: 0;
        padding: 0;
        height: 50px;
    }
    
</style>