<Plans/>
<Footer/>
<script>
    import Plans from '../components/PricingSection/plans.svelte'
    import Footer from "../components/PricingSection/footer.svelte";
</script>

<style lang="scss">
    :global(*)
    {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
    :global(body)
    {
        background: $bg-l;
        color: #111;
        transition: $theme-fade;
        overflow-x: hidden;
        font-family: $font;
    }
    :global(.blue)
    {
        color: $blue;
    }
    :global(.orange)
    {
        color: $orange;
    }
    :global(h1, h2, h3, h4, h5, h6)
    {
        font-family: $headline !important;
    }
</style>
