<script>
    import Section from '../components/Section.svelte';
    import Main from '../components/Main.svelte';
    import Chart from '../components/Chart.svelte';

    // background: radial-gradient(circle, rgba(52,80,223,1) 0%, rgba(127,64,204,1) 100%);
    // background: radial-gradient(circle, rgba(121,52,223,1) 0%, rgba(64,123,204,1) 100%);
</script>

<Main>
    <Section
        clr="radial-gradient(circle, rgba(52,80,223,1) 0%, rgba(127,64,204,1) 100%)"
        cp="ellipse(75% 100% at 31.5% 0%)"
        mediaSmall="true"
    >
        <Chart />
    </Section>
    <Section />
</Main>

<style lang="scss">
</style>
