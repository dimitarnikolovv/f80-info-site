<script>
    import {link} from 'svelte-spa-router'
    import active from 'svelte-spa-router/active';
    import ArrowRight from './icons/ArrowRight.svelte';

</script>

<nav>
    <ul>
        <li><a href="/" use:link use:active={'/'}>Home</a> 
            <div class="arrow">
                <ArrowRight url='/'/>
            </div>
        </li>
        <li><a href="/about" use:link use:active={'/about'}>About</a>
            <div class="arrow">
                <ArrowRight url='/about'/>
            </div>
        </li>
        <li><a href="/contact" use:link use:active={'/contact'}>Contact</a>
            <div class="arrow">
                <ArrowRight url='/contact'/>
            </div>
        </li>
</nav>

<style lang="scss">
    :global(a.active){
        color: white;
    }

    ul{
        display: flex;
        gap: 1rem;
        
        li{
            font-weight: 500;
            font-style: normal;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 0.5rem;
            height: 2rem;
            color: #aaa;
            background-color: #5f7d95;
        }

        a{
            padding-inline-start: 0.4rem;
            transition: color 200ms ease-in-out;
        }
    }
</style>