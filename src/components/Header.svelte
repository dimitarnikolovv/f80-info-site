<script>
    import Nav from './Nav.svelte';
    import F80Logo from './icons/F80Logo.svelte';
</script>

<header>
    <div class="container">
        <F80Logo />
        <Nav />
    </div>
</header>

<style lang="scss">
    header {
        position: relative;
        width: 100vw;
        padding-block: 1rem;
        background-color: transparent;
        div.container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 4rem;
            max-width: 90vw;
            margin-inline: auto;
        }
    }

    header:global(.fixed) {
        background-color: var(--clr-primary-700);
    }
</style>
