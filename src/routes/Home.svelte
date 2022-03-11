<script>
    import Section from '../components/Section.svelte';
</script>

<Section>
    <h1>Lorem ipsum <span class="text-modifier">lorem ipsum</span> dolor sit</h1>
</Section>

<style lang="scss">
    span.text-modifier {
        font-weight: 600;
    }
</style>
