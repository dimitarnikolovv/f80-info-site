<script>
    import Section from '../components/Section.svelte';
    import Main from '../components/Main.svelte';
    import Car from '../components/icons/Car.svelte';

    // background: radial-gradient(circle, rgba(52,80,223,1) 0%, rgba(127,64,204,1) 100%);
    // background: radial-gradient(circle, rgba(121,52,223,1) 0%, rgba(64,123,204,1) 100%);
</script>

<Main>
    <Section
        clr="radial-gradient(circle, rgba(58,175,169,1) 0%, rgba(43,122,120,1) 100%)"
        cp="ellipse(75% 100% at 31.5% 0%)"
        mediaSmall="true"
    >
        <h1 class="heading-light">
            Каква е <span class="text-modifier">нашата</span> цел?
        </h1>
        <div class="text-wrapper">
            <div class="left-child">
                <p>
                    Глобалната цел на проекта е да се създаде единна среда за комуникация между
                    автономни автомобили, като се включат и автомобили с шофьор като преходен
                    период. В зависимост от пътните условия софтуерът самостоятелно преценя и
                    контролира трафика, без да се нуждаем от светофари, като се избягва и човешка
                    грешка. Такъв тип компютърна система трябва да бъде стандартизирана от
                    регулаторните органи по света, за да се създаде безопасност и улеснение при
                    пътуване.
                </p>
            </div>
            <div class="right-child">
                <Car />
            </div>
        </div>
    </Section>

    <Section>
        <h1 class="heading-dark">
            Lorem, ipsum dolor <span class="text-modifier">lorem</span> porem, ipsum
        </h1>
    </Section>

    <Section
        clr="radial-gradient(circle, rgba(58,175,169,1) 0%, rgba(43,122,120,1) 100%)"
        cp="ellipse(168% 100% at 144.4% 100%)"
    >
        <h1 class="heading-dark">
            Lorem ipsum <span class="text-modifier">lorem ipsum</span> dolor sit
        </h1>
    </Section>

    <Section
        clr="radial-gradient(circle, rgba(58,175,169,1) 0%, rgba(43,122,120,1) 100%)"
        cp="ellipse(279% 100% at -162.97% 0%)"
    >
        <h1 class="heading-light">
            Lorem, ipsum dolor <span class="text-modifier">lorem</span> porem, ipsum
        </h1>
    </Section>
</Main>

<style lang="scss">
    span.text-modifier {
        font-weight: 600;
    }

    .heading-light {
        color: #def2f1;
    }

    .heading-dark {
        color: #17252a;
    }

    div.text-wrapper {
        position: relative;
        display: flex;
        gap: 2rem;

        div {
            width: 50%;
        }

        p {
            color: inherit;
            font-size: 1.2rem;
            line-height: 1.2em;
            font-weight: 400;
        }

        @media only screen and (max-width: 768px) {
            flex-direction: column;
            div {
                width: 90vw;
            }
        }
    }
</style>
