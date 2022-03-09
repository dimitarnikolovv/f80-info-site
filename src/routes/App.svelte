<script>
    import Footer from '../components/Footer.svelte'
    import Header from '../components/Header.svelte'
    import Router from 'svelte-spa-router';
    import Home from './Home.svelte';
    import About from './About.svelte';
    import Contact from './Contact.svelte'
    import NotFound from './NotFound.svelte';

    let routes = {
        '/': Home,
        '/about': About,
        '/contact': Contact,

        '*': NotFound,
    }
</script>

<Header/>

<main>
    <Router {routes}/>
</main>

<Footer/>

<style lang="scss">
    main{
        background-color: cadetblue;
        display: flex;
        justify-content: center;
        align-items: center;
        width: 100vw;
    }
</style>