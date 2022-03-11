<script>
    export let clr = 'white';
</script>

<section style="background-color: {clr}">
    <div class="container">
        <slot />
    </div>
</section>

<style lang="scss">
    section {
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 1rem;
        width: 100vw;
    }
</style>
