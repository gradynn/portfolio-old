<script>
    import projects from './projects.json';
    import Project from './project.svelte';
</script>

<style>
    .blog-container {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 100%;
    }

    .section-header {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        margin: 1rem;
    }

    .primary-heading {
        font-size: 4rem;
        margin: 0;
    }
    
    .quote {
        display: flex;
        flex-direction: column;
        align-items: end;
        justify-content: center;
        margin: 1rem;
    }
    
    .secondary-heading {
        margin: 0;
    }
</style>

<div class="blog-container">
    <div class="section-header">
        <p class="primary-heading">Projects</p>
        <div class="quote">
            <p class="secondary-heading">What I cannot create, I do not understand.</p>
            <p class="secondary-heading">- Richard Feynman</p>
        </div>
    </div>
    {#each projects as project}
        <Project {...project} />
    {/each}
</div>
