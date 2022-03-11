<script>
    import Nav from './Nav.svelte';
    import Logo from './icons/Logo.svelte';
</script>

<header>
    <Logo />
    <Nav />
</header>

<style lang="scss">
    header {
        position: relative;
        display: flex;
        justify-content: center;
        align-items: center;
        width: 100vw;
        height: 4rem;
        padding-block: 1rem;
        background-color: transparent;
    }

    header:global(.fixed) {
        background-color: var(--clr-primary-700);
    }
</style>
