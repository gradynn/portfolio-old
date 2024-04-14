<script lang="ts">
    export let imageUrl: string;
    export let title: string;
    export let previewText: string;
    export let article: string = '';
    export let isActive: boolean = false;
</script>

<style lang="scss">

.project-bubble {
        display: flex;
        flex-direction: row;
        align-items: center;
        width: 75%;
        height: 300px;
        margin: 1rem;
        padding: 1rem;
        border-radius: 10px;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    .project-bubble img {
        width: 50%;
        height: 100%;
        object-fit: cover;
        border-radius: 10px;
    }

    .project-bubble h3 {
        margin: 0.5rem 0;
    }

    .project-bubble p {
        margin: 0.5rem 0;
    }

    .project-bubble a {
        margin: 0.5rem 0;
        padding: 0.5rem 1rem;
        border-radius: 5px;
        background-color: color('primary');
        color: white;
        text-decoration: none;
    }

</style>

<div class="project-bubble">
    <img src={imageUrl} alt={title} />
    <h3>{title}</h3>
    <p>{previewText}</p>
</div>
{#if isActive}
    <div>
        <p>{@html article}</p>
    </div>
{/if}