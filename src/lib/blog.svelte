<script>
    import projects from './projects.json';
</script>

<style>
    .blog-container {
        display: flex;
        flex-direction: column;
        justify-content: center;
        width: 100%;
    }

    .project-bubble {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        width: 75%;
        height: 300px;
        margin: 1rem;
        padding: 1rem;
        border-radius: 10px;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    .project-bubble img {
        width: 100%;
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

<div class="blog-container">
    {#each projects as project}
        <div class="project-bubble">
            <img src={project.imageUrl} alt={project.title} />
            <h3>{project.title}</h3>
            <p>{project.previewText}</p>
            <a href={project.link}>Read More</a>
        </div>
    {/each}
</div>
