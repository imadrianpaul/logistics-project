<script>
    export let icon;
    export let title="";
    export let description="";
</script>

<div class="features">
    <div class="features-content">
        {#if icon}
        <span class ="features-icon">{icon}</span>
        {/if}
        <h2 class="features-title">{title}</h2>
        <p class="features-description">{description}</p>
    </div>
</div>

<style>

    .features {

        max-width: 600px;
        overflow: hidden;

    }

    .features-content {

        padding: 1rem;

    }

    .features-icon {
        font-size: 2rem;
        color: #fea238;
        margin-bottom: 0.5rem;
    }

    .features-title {
        font-size: 24px;
        margin: 0.5rem 0;
        color: rgb(127, 91,23);
    }

    .features-description {
        font-size: 0.9rem;
        color: #666;
    }

</style>