<script>
    export let title = "";
    export let subtitle = "";
    export let description = "";
    export let description2 = "";
</script>

<div class="card">
    <div class="card-content">
        <h2 class="card-title">{title}</h2>
        <h3 class="subtitle">{subtitle}</h3>
        <p class="card-description">{description}</p>
        <p class="card-description2">{description2}</p>
        <slot name="actions"></slot>
    </div>
</div>

<style>
    
    .card {
        max-width: 300px;
        border-radius: 8px;
        overflow: hidden;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        background-color: #fea238;
        transition: transform 0.2s;
    }

    .card:hover {
        transform: translateY(-5px);
    }

    .card-content {
        padding: 1rem;
    }

    .card-title {
        font-size: 1.25rem;
        margin: 0.5rem 0;
        color: #333;
    }

    .card-description {
        font-size: 0.9rem;
        color: #666;
    }

    .card-description2 {
        font-size: 0.9rem;
        color: #666;
    }
    
</style>