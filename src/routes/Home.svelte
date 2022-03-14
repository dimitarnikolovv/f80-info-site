<script>
    import { slide } from 'svelte/transition';
    import Section from '../components/Section.svelte';
    import Main from '../components/Main.svelte';

    // background: radial-gradient(circle, rgba(52,80,223,1) 0%, rgba(127,64,204,1) 100%);
    // background: radial-gradient(circle, rgba(121,52,223,1) 0%, rgba(64,123,204,1) 100%);
</script>

<Main>
    <Section
        clr="radial-gradient(circle, rgba(52,80,223,1) 0%, rgba(127,64,204,1) 100%)"
        cp="ellipse(75% 100% at 31.5% 0%)"
        mediaSmall="true"
    >
        <h1>Lorem ipsum <span class="text-modifier">lorem ipsum</span> dolor sit</h1>
        <div class="text-wrapper">
            <div class="left-child">
                <p>
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Iusto tempora, magni
                    neque tempore fugiat voluptas quas harum sint porro consequuntur delectus
                    excepturi maiores, beatae, minus placeat quo fugit. Aliquam ullam sequi,
                    consectetur, aspernatur iure veniam pariatur dignissimos similique mollitia iste
                    quas sapiente labore itaque voluptate molestias quibusdam excepturi consequatur
                    inventore perferendis dolorum dicta iusto autem incidunt! Aspernatur ducimus
                    repudiandae, deserunt consequatur, rerum aliquam ullam nulla cum nemo molestias
                    sint corporis officia id porro debitis iusto eligendi modi iure odio doloribus
                    voluptas culpa maiores perferendis. Fugit doloremque consequatur veniam ducimus
                    eveniet non, voluptate ab tempora vitae omnis nostrum libero eaque nobis ipsa
                    aliquam totam veritatis similique quidem minima corporis labore at culpa. At
                    similique veritatis aperiam nihil ipsam doloremque hic repudiandae.
                </p>
            </div>
            <div class="right-child">
                <p>
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Similique quae neque
                    impedit itaque soluta error inventore vel alias molestias facere atque ipsum,
                    natus odit quia, magni temporibus reprehenderit, aut odio vero sequi nemo fuga
                    nisi! Repellat amet consequuntur nisi eligendi!
                </p>
            </div>
        </div>
    </Section>

    <Section>
        <h1>Lorem, ipsum dolor <span class="text-modifier">lorem</span> porem, ipsum</h1>
    </Section>

    <Section
        clr="radial-gradient(circle, rgba(121,52,223,1) 0%, rgba(64,123,204,1) 100%)"
        cp="ellipse(168% 100% at 144.4% 100%)"
    >
        <h1>Lorem ipsum <span class="text-modifier">lorem ipsum</span> dolor sit</h1>
    </Section>

    <Section
        clr="radial-gradient(circle, rgba(121,52,223,1) 0%, rgba(64,123,204,1) 100%)"
        cp="ellipse(279% 100% at -162.97% 0%)"
    >
        <h1>Lorem, ipsum dolor <span class="text-modifier">lorem</span> porem, ipsum</h1>
    </Section>
</Main>

<style lang="scss">
    span.text-modifier {
        font-weight: 600;
    }

    div.text-wrapper {
        position: relative;
        display: flex;
        gap: 2rem;

        div {
            width: 50%;
        }

        @media only screen and (max-width: 768px) {
            flex-direction: column;
            div {
                width: 90vw;
            }
        }
    }
</style>
