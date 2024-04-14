<style lang="scss">
    .container {
        width: calc(100% - 2rem);
        height: calc(100vh - 2rem);
        border: 0.2rem solid #0b0d32;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        color: #0b0d32;
        position: relative; 
        padding: 1rem; 
        box-sizing: border-box; 
    }

    .name, .subtitle, .phone, .description {
        margin: 0; 
        position: static; 
    }

    .name {
        font-size: 5rem;
    }

    .subtitle {
        font-size: 2rem;
    }

    .phone {
        position: absolute; 
        top: 0.5rem; 
        left: 1rem; 
        font-size: 3rem; 
    }

    .description {
        position: absolute; 
        bottom: 1rem; 
        font-size: 2rem; 
    }
</style>

<div class="container">
    <p class="name">GRADYN NAGLE</p>
    <p class="subtitle">Full Stack Software Engineer</p>
    <p class="phone">510-219-1647</p>
    <p class="description">University of California, Davis | B.S. Computer Science | email gnagle@ucdavis.edu</p>
</div>
