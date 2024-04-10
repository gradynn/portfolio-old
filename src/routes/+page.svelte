<script lang='ts'>
    let scrollTop = 0;
    function handleScroll(event: UIEvent) {
      scrollTop = (event.target as Element).scrollTop;
    }
</script>

<style lang='scss'>
.child {
    height: 100vh;
    width: 100%;
    scroll-snap-align: start;
    margin: 0;
    box-sizing: border-box;
}
</style>

<div>
    <section class="child">
        Section 1
    </section>
    <section class="child">
        Section 2
    </section>
    <section class="child">
        Section 3
    </section>
</div>