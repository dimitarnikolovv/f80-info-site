<script>
    import {link, location} from 'svelte-spa-router'
    import active from 'svelte-spa-router/active';
    import ArrowRight from './icons/ArrowRight.svelte';


$: isActive = function(url) {
    return (url === $location) ? true : false;
}

</script>

<nav>
    <ul>
        <li><a href="/" use:link use:active={'/'}>Home</a> 
            <div class="arrow">
                <ArrowRight active={isActive('/')}/>
            </div>
        </li>
        <li><a href="/statistics" use:link use:active={'/statistics'}>Statistics</a>
            <div class="arrow">
                <ArrowRight active={isActive('/statistics')}/>
            </div>
        </li>
        <li><a href="/contact" use:link use:active={'/contact'}>Contact</a>
            <div class="arrow">
                <ArrowRight active={isActive('/contact')}/>
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
            // background-color: #5f7d95;

            div{
                transition: transform 200ms ease-in-out;
            }
        }

        a{
            padding-inline-start: 0.4rem;
            transition: color 200ms ease-in-out;

            &:hover{
                & + div{
                        transform: translateX(5px);
                }
            }
        }
    }
</style>