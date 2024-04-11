<script lang='ts'>
    import { onMount } from 'svelte';

    import Blog from '$lib/blog.svelte';
    import Profile from '$lib/profile.svelte';
</script>

<style lang='scss'>
.child {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    scroll-snap-align: start;
    margin: 0;
    box-sizing: border-box;
}

#profile {
    height: 100vh;
    width: 100%;
}

.menu-wrapper {
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 100;
}

.primary-heading {
    font-size: 4rem;
    border-bottom: 1px solid color('primary');
}

</style>

<div>
    <section id="profile" class="child">
        <Profile />
    </section>
    <section id="projects" class="child">
        <h1 class="primary-heading">Projects</h1>
        <Blog />
    </section>
</div>