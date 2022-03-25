<script>
    import Header from '../components/Header.svelte'
    import CustomerData from '../components/CustomerData.svelte'
    import NoCode from '../components/NoCode.svelte'
    import ExternalSystems from '../components/ExternalSystems.svelte'
    import Possible from '../components/Possible.svelte'
    import Launch from '../components/Launch.svelte'
    import Database from '../components/Database.svelte';
    import Footer from '../components/Footer.svelte';
</script>

<Header />
<CustomerData />
<NoCode />
<ExternalSystems/>
<Possible/>
<Launch/>
<section class="outer-container">
    <Database/>
    <Footer />
</section>

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
        min-height: 500vh;
    }
    :global(.blue)
    {
        color: $blue;
    }
    :global(.orange)
    {
        color: $orange;
    }
    .outer-container 
    {
        background-image: linear-gradient(to bottom, $blue 30%, rgb(255, 94, 148));
    }
</style>
